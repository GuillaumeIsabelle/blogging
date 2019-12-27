---
ID: 1352
post_title: POP Collision Behavior
author: gicomadmin
post_excerpt: ""
layout: post
permalink: >
  http://guillaumeisabelle.com/blogging/2019/12/27/pop-collision-behavior/
published: true
post_date: 2019-12-27 11:13:21
---
> The POP Collision Behavior node performs operations based on collisions set in the hit attributes.

Source: *[POP Collision Behavior][1]*

<!-- wp:paragraph -->

Typically, the [POP Collision Detect][2] node is used to do both the collision detection and resolution. However, this node can be useful when responding to DOP collisions created by the **Add Hit Attributes**option of the [POP Solver][3].

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

This operator modifies the `P`, `Cd`, `stopped`, `stuck`, `sliding`, `pospath`, `posuv`, and `posprim` attributes.

<!-- /wp:paragraph -->

 [1]: https://www.sidefx.com/docs/houdini/nodes/dop/popcollisionbehavior.html
 [2]: https://www.sidefx.com/docs/houdini/nodes/dop/popcollisiondetect.html
 [3]: https://www.sidefx.com/docs/houdini/nodes/dop/popsolver.html