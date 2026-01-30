# Deep-Learning-exam
Infix-to-postfix translation

The purpose of this project is to implement a neural network that performs the translation of mathematical formulae from traditional infix notation - where the operator appears between two operands - to postfix notation (also known as Reverse Polish Notation), where the operator follows the operands.

Infix notation is the most commonly used in human-readable mathematics (e.g., a + b), but it is inherently ambiguous without additional syntactic aids such as parentheses or operator precedence rules. This ambiguity arises because different parse trees can correspond to the same expression depending on how operations are grouped.

In contrast, postfix notation eliminates the need for parentheses entirely. The order of operations is explicitly encoded by the position of the operators relative to the operands, making it more suitable for stack-based evaluation and easier to parse programmatically.

Example. Consider the ambiguous infix expression: a + b * c

This expression can be parsed in at least two different ways:

Interpretation (Infix): (a + b) * c    

Equivalent Postfix: ab+c*

Interpretation (Infix): a + (b * c)           

Equivalent Postfix: abc*+

This project aims to learn such disambiguations and generate the correct postfix form from a given infix expression using a data-driven approach based on neural networks. To simplify the task and control the complexity of expressions, we restrict our dataset to formulae with a maximum syntactic depth of 4. This means that the abstract syntax trees representing these expressions will have at most four levels, ensuring that the neural network operates on a bounded and manageable set of possible structures.
