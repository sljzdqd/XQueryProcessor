# XQueryProcessor
https://cseweb.ucsd.edu/classes/wi20/cse232B-a/
Milestones 1 and 2 (Naïve Evaluation) [due in weeks 4 and 7, respectively]: A straightforward query execution engine receives the simplified XQuery and an input XML file and evaluates the query using a recursive evaluation routine which, given an XQuery expression (path, concatenation, element creation, etc) and a list of input nodes, produces a list of output nodes. For the XQuery parser, we recommend the ANTLR4. Provided with a grammar, ANTLR generates a compiler which automatically constructs abstract syntax trees of  its input expressions.
Milestone 1 delivers a naive evaluator for XPath, while Milestone 2 extends it to XQuery.

Milestone 3 (Efficient Evaluation): Implement a join operator as defined in this note. Implement an algorithm which detects the fact that the FOR and WHERE clause computation can be implemented using the join operator. You may assume that the input XQueries to be optimized are in the simplified syntax given in the note. No need to first normalize your queries to this form.
