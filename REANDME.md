# REANDME

Milestones 1 and 2 (Naïve Evaluation) [due in weeks 4 and 7, respectively]: A straightforward query execution engine receives the simplified XQuery and an input XML file and evaluates the query using a recursive evaluation routine which, given an XQuery expression (path, concatenation, element creation, etc) and a list of input nodes, produces a list of output nodes. For the XQuery parser, we recommend the ANTLR4. Provided with a grammar, ANTLR generates a compiler which automatically constructs abstract syntax trees of  its input expressions.
Milestone 1 delivers a naive evaluator for XPath, while Milestone 2 extends it to XQuery.

Milestone 3 (Efficient Evaluation): Implement a join operator as defined in this note. Implement an algorithm which detects the fact that the FOR and WHERE clause computation can be implemented using the join operator. You may assume that the input XQueries to be optimized are in the simplified syntax given in the note. No need to first normalize your queries to this form.
- The source codes are under the src/ directory.

- The XQueryProcessor.jar is the exported jar file. It can be executed as this:

  1. Enter the directory that contains the jar, for example

     `cd XQueryProcessor/`

  2. Execute a command like this:

     `java -jar XQueryProcessor.jar 'doc("j_caesar.xml")//(ACT,PERSONAE)/TITLE'`

     Reminder: the input query should be enclosed in single quotes, otherwise there will be a syntax error.

  3. Then there will be outputs in the terminal.
