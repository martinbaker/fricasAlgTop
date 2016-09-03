Algebraic Topology for FriCAS Program
-------------------------------------
Since release 1.3.0 the algebraic topology code is now included in the FriCAS library.

However there are some outstanding issues to be sorted out, see thread here:
https://groups.google.com/forum/?hl=en#!topic/fricas-devel/8GFaGT9ON6E
I have therefore created this repository to facilitate discussion of the improvements needed.

Included here are:

<ul>
  <li>algebraictopology.spad</li>
  <li>gpresent.spad</li>
  <li>logic.spad</li>
</ul>

algebraictopology.spad
----------------------

This includes simplicial complexes and cubical complexes.

For further information see the documentation here:<ul>
  <li>http://www.euclideanspace.com/prog/scratchpad/mycode/topology/simplex/</li>
  <li>http://www.euclideanspace.com/prog/scratchpad/mycode/topology/cubical/</li>
</ul>

gpresent.spad
-------------

Group represented by its generators and relations.
Here we use it to hold homotopy group such as fundamental group.

For further information see the documentation here:
http://www.euclideanspace.com/prog/scratchpad/mycode/discrete/finiteGroup/presentation/

logic.spad
----------

Includes various logic related structures including partial order, lattice structures

I have also moved intuitionistic logic here from computation.spad

Since I last mentioned this on the forum I was kindly sent some unpublished code (related to Moebius function) by Franz Lehner with permission to merge this with my own poset related code. This is now all included in the code on Github.

These are my notes related to the code written by Franz:
http://www.euclideanspace.com/prog/scratchpad/mycode/discrete/logic/moebius/

I have included Logic category, this is the same as existing Logic
category in Boolean.spad as it is intended to replace it. Since this
category is more general than just Boolean I thought it more appropriate
to put it in logic.spad. 

For further information see the documentation here:<ul>
  <li>http://www.euclideanspace.com/prog/scratchpad/mycode/discrete/logic/</li>
  <li>http://www.euclideanspace.com/prog/scratchpad/mycode/discrete/logic/moebius/</li>
</ul>

TODO
----
There is a lot more work to be done on this code but I think it is in a state where it can be of some use to others. If it is included in the FriCAS library then there is always a chance that someone else may be able to help. I would welcome as much help as I can get.

Some improvements I would like to make at some time in the future are:

1) I would like to fully implement the geometric version of simplicial complex. One reason is that I would like to make it the standard way to represent 2D, 3D and n-dimensional shapes in code such as scene.spad. So the shapes can be transformed and output in various ways however they would have better mathematical properties than the structures usually used to represent shapes in computer science. This would involve writing code to test for overlapping simplexes and so on.

2) The code that Franz Lehner sent to me also included isomorphism testing and drawing (using algorithms from Freese's book on "Free Lattices"). I would like to merge this with my code. (it may not all be generalisable to graphs/complexes but parts of it may be and the remainder can still be used for posets).



