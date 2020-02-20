---
ID: 1684
post_title: MantaFlow / General Concepts
author: gicomadmin
post_excerpt: ""
layout: post
permalink: >
  http://guillaumeisabelle.com/blogging/2020/02/20/mantaflow-general-concepts/
published: true
post_date: 2020-02-20 14:28:22
---
#  General Concepts The aim of this section is to provide some insights about general design choices of the mantaflow code. 

*   All simulations use normalized spatial coordinates. Thus a cell always has size one. This shifts complexity into the scene setups, but prevents numerical problems in the simulation, and improves readbility of the values you'll encounter in a simulation.
*   The objects of a simulation should have as little internal state as possible. All this info should be represented in the Python scene.
*   We've tried to keep the feature set as small as possible, to avoid feature creep, and to keep the code size down. Also, we've tried to minimize the use of external libraries. The most crucial dependence at the moment is <tt>Python</tt>. Instead of strictly following an object oriented design, with a nice class hierarchy etc., mantaflow takes a data centric view. A fluid solver can be seen as a collection of operators working on different Eulerian or Lagrangian variables. As such, grids and particles are the central data types of all mantaflow scenes. The main goal of this design is to keep things as simple as possible. Each of the grids and particle data fiels supports Scalar values (int or Real), and small vectors (three or four dimensional). Support for 4D data is intentionally different from 3D data. Usually, 3D data will be sufficient for most solvers. 2D is seen as a special case of 3D in mantaflow, thus code is shared, and all 3D code should work with 2D. The 4D handling is different: 

*   scenes are still usually mostly 3D, but can work with additional 4D data on the side.
*   The interfaces are structured in the same way for 3D and 4D grids, so operators can still be made to work with both using templates.
*   If 4D operators are needed in a scene, 4D support (and the size of the time dimension) can be manually enabled with the <tt>fourthDim</tt>.
*   As before, grid dimensions are constant for all grids of a solver, thus within a single solver as parent, all 4D grids will have the same size of the <tt>t</tt> dimension.