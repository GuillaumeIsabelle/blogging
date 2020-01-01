---
ID: 1425
post_title: Gas Surface Tension
author: gicomadmin
post_excerpt: ""
layout: post
permalink: >
  http://guillaumeisabelle.com/blogging/2020/01/01/gas-surface-tension/
published: true
post_date: 2020-01-01 04:51:03
---
> A microsolver that calculates a surface tension force proportional to the curvature of the surface field. The Gas Surface Tension DOP is a microsolver used in building larger fluid simulations. The <a class="link   Node" title="A solver for Sign Distance Field (SDF) liquid simulations." href="https://www.sidefx.com/docs/houdini/nodes/dop/fluidsolver.html">Fluid Solver</a> and <a class="link   Node" title="Sets and configures a Smoke solver. This is a slightly lower-level solver that is the basis for the Pyro solver." href="https://www.sidefx.com/docs/houdini/nodes/dop/smokesolver.html">Smoke Solver</a> DOPs that allow microsolvers to be added before or after the main solver step to extend or tweak the simulation. Alternatively, enterprising people may attempt to build an entire new solver out of microsolvers. The Gas Surface Tension DOP calculates a surface tension force and applies it to the velocity field. The force is present at the surface boundary and is proportional to the curvature of the surface. The effect is to push in on pimples and push out on dimples, thereby flattening the surface. Source: *[Gas Surface Tension][1]*

 [1]: https://www.sidefx.com/docs/houdini/nodes/dop/gassurfacetension.html