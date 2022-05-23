# The Maximum density still life

The Maximum Density Still Life Problem (CSPLib prob032) is to find the maximum number
of live cells that can fit in an n × n region of an infinite board, so that the board is stable
under the rules of Conway’s Game of Life. It is considered a very difficult problem and
has a raw search space of O (2^n^2). Previous state of the art methods could only solve
up to n = 20. We give a powerful reformulation of the problem into one of minimizing
“wastage” instead of maximizing the number of live cells. This reformulation allows us
to compute very strong upper bounds on the number of live cells, which dramatically
reduces the search space. It also gives us significant insights into the nature of the problem.
By combining these insights with several powerful techniques: remodeling, lazy clause
generation, bounded dynamic programming, relaxations, and custom search, we are able
to solve the Maximum Density Still Life Problem for all n. This is possible because the
Maximum Density Still Life Problem is in fact well behaved mathematically for sufficiently
large n (around n > 200) and if such very large instances can be solved, then there exist
ways to construct provably optimal solutions for all n from a finite set of base solutions.
Thus we show that the Maximum Density Still Life Problem has a closed form solution and
does not require exponential time to solve
