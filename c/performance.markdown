Ars - C Performance
===================
1. Arrange code for contiguous basic blocks and eliminate unnecessary branches.
    * Reasoning:
        * Compilers generate code as if reading from top to bottom
    * Utilizing:
        * Code as if reading a written text.

2. Arrange code to be consistent with branch prediction:
    * Reasoning:
        * Given no other information all conditionals are treated as equal.
    * Utilizing:
        * First and default branches are considered common paths.
        * Use \_\_builtin\_expect.

3. Arrange code with two or more common path and conditionals within into a tree,
   peel common paths
    * Reasoning:
        * Reduces branch misprediction.
    * Utilizing:
        * Convert nested if statments into a tree.
        * Peel common paths outside of tree

4. Arrange structures for sequential access.
    * Reasoning:
        * Prefetching is based on sequential access.
    * Utilizing:
        * Write structures based on most used elements to least.

5. Arrange structures so that they are aligned to a natural operand size boundary.
    * Reasoning:
        * Removes padding.
    * Utilizing:
        * Write structures from smallest type to largest type and group.

6. Arrange code so data dependence is minimal.
    * Reasoing:
        * Allows more instruction level parallelism
    * Utilizing:
        * Write code with out dependence on previous variables.
