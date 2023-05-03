Download Link: https://assignmentchef.com/product/solved-cs-570-programming-foundations-programming-assignment-8
<br>
<strong> </strong>You are asked to develop a program that uses the stack data structure to check for balanced parentheses in an arithmetic expression. Specifically, consider the problem of checking to see if an arithmetic expression involving three kinds of parentheses is a proper expression in that the parentheses are balanced in pairs. For example,




(6 + {[2+7]*9}/8)




is a proper expression. We will be concerned with three kinds of parentheses:




<ul>

 <li>Curved ( ) often called simply parentheses</li>

 <li>Curly { } called braces</li>

 <li>Square [ ] called brackets</li>

</ul>




We will call all of these parentheses.




First, create a text file with 20 examples of proper and improper expressions. You may assume that there is one expression per line in the input file. You may also assume that the arithmetic parts of each expression, those that do not involve parentheses, for example 25 * 5 are all proper. So you will never see things like (+ 25 * 2 ). Your input file might look like this:




(25 * 5) * [{45 / 2} – 500]

(((50 / 7))

… etc




For each of the expressions in the input file your program should assess if the expression is proper or improper and produce an output file with either the word “proper” or “improper” next to each expression from the input file. For example, your output file for the above input file will look like this:




(25 * 5) * [{45 / 2} – 500]        proper

(((50 / 7))         improper

…




Here is a hint. You should store each expression into a string variable. To check whether or not an expression is proper, scan the string from left to right, pushing each left (opening) parenthesis we encounter onto a stack. When a right parenthesis is encountered, we pop an entry from the stack and it should match the right parenthesis in type. For example, ( matches with ), { matches with }, or [ matches with ]. If it does not match, the expression is not a proper one because the parentheses are not balanced. With a proper expression, the stack of the left parentheses should be empty when we reach the end of the expression.





