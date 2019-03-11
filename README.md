# Bidirected-Search-on-Permutation
Bidirected Search permutation - description, mathematical proof and Code implementation in Python

The concept of a permutation has numerous applications in computer science, for example, in the analysis of sorting algorithms and in implementations of distributed systems.

Formally, a permutation is a bijection from a set onto itself. For simplicity, let us restrict ourselves to the sets [n] := f1; 2; : : : ; ng of the rst n positive integers, and denote by Sn the set of all permutations on [n]. It is often convenient to represent a permutation by the n-tuple ( (1); (2); : : : ; (n)).

Swapping two elements of a permutation yields another permutation. For i; j 2 [n] let Tij : Sn ! Sn be the mapping that swaps the images of i and j, that is, if 2 Sn, then := Tij ( ) is given by (i) = (j), (j) = (i), and (k) = (k) if i 6=k 6=j.

Example.	Let	= (2; 4; 3; 1). Then T13( ) = (3; 4; 2; 1).

Now, consider allowing only swaps with some pairs (i; j). For any integer d	0, let

 
Pd :=  (i; j) 2 [n]	[n] : i = j or d	j	i	n	d :

Say that a permutation is (d; `)-reachable from if there are (i1; j1); (i2; j2); : : : ; (i`; j`) 2 Pd such that the corresponding swaps transform to , that is, = Ti`j` Ti2j2 Ti1j1 ( ).

The topic can be well understood by solving the following three questions . This repository provides the comprehensive solutions to these problems which were asked in a university assignment. 

1.

Prove that for any positive integer n, the permutation (n; n  1; : : : ; 1) is (1; bn=2c)-

reachable from (1; 2; : : : ; n).

2.	

To  nd out whether   is (d; `)-reachable from  , one may apply bidirected search as

follows: First generate all permutations that are (d; b`=2c)-reachable from . Next generate all permutations that are (d; d`=2e)-reachable from . Finally, report \YES" if the two generated sets intersect, and otherwise report \NO".

Describe the algorithm using pseudocode; in particular, describe how the sets of per-mutations are generated. (You may assume the given arguments are valid: you need not implement error handling.)

3.	
Implement the algorithm of the previous task using one of the following programming languages (using only standard libraries): C, C++, Java, Python. Show your code.

Use your implementation to solve, for all d = 1; 2; : : : ; 4 and ` = 1; 2; : : : ; 9, whether

(9; 8; : : : ; 1) is (d; `)-reachable from (1; 2; : : : ; 9). Show the results as a 4  9 matrix.


