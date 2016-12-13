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

Includes various logic related structures including partial order, lattice structures.
I have also moved intuitionistic logic here from computation.spad

Logic is related to Topology as discussed in Steven Vickers book 'Topology via Logic'. I would like to encode this computationally, that is define topology using lattice structures.

For further information see the documentation here:<ul>
  <li>http://www.euclideanspace.com/prog/scratchpad/mycode/discrete/logic/</li>
  <li>http://www.euclideanspace.com/prog/scratchpad/mycode/discrete/logic/moebius/</li>
</ul>

TODO
----

Some improvements I would like to make at some time in the future are:

1) I would like to fully implement the geometric version of simplicial complex. One reason is that I would like to make it the standard way to represent 2D, 3D and n-dimensional shapes in code such as scene.spad. So the shapes can be transformed and output in various ways however they would have better mathematical properties than the structures usually used to represent shapes in computer science. This would involve writing code to test for overlapping simplexes and so on.

2) The code that Franz Lehner sent to me also included isomorphism testing and drawing (using algorithms from Freese's book on "Free Lattices"). I would like to merge this with my code. (it may not all be generalisable to graphs/complexes but parts of it may be and the remainder can still be used for posets).

Related Code
------------
<ul>
  <li>https://github.com/martinbaker/multivector</li>
  <li>https://github.com/martinbaker/fricasScene</li>
  <li>https://github.com/fricas/fricas</li>
</ul>




