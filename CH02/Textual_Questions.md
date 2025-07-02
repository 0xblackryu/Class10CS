---
layout: default
title: CH02 Textual Questions
---
# REVIEW QUESTIONS AND EXERCISES
1. What is a constant? Explain the constants in C. <br>
    Ans : Any unchanged value in a program during the program execution is called constant.<br>
     In C language, constant are divided into two types Numeric and String or character :<br> 
     1. Numeric Constant :<br>
            i.Integer constant : an integer constant is a signed or unsigned whole number.<br> 
                    eg. -23,12,+240.<br>
           ii.Real or Floating point constant : Any signed or unsigned number with fractional part is called real or floation point constant.<br>
                    eg. -23.41, +234.21,3.14<br>
        
    2.String or character constant : <br>
            i.Single character string constant : any letter or character enclosed in single apostrophe is called single character string constant.<br>
                    eg. 'a','$','+'.<br>
           ii.String og characters constant : any string of characters consisting of letters, digits and symbols enclosed in double quotes is called string of characters constant.<br>
                   eg. "Some Names", "India +91","$$Money".

2. What is a variable? How are the variables declared in C?<br>
Ans : A variable is an identifier or a name which is used to refer to a value and this value varies or changes during the program execution.Variabe used in a C program are declared with appropriate datatypes along with their name.


3. What is an expression? What are the operators in C? <br>

Ans : An expression consists of variable and constants seperated by operators.

4. What is a library function? Mention its use. <br>

Ans : Library functions are the build in program that are available with the compiler.It is used to perform standard mathematical operations. <br>
        eg. sqrt(),fabs(), log(),etc.

5. Convert the following mathematical expressions into C expressions. <br>
(i) $\frac{a+b}{c+d}$ <br>
(ii) $\frac{ab}{c^2+d}g$ <br>
(iii) $\sqrt{1+x}\frac{\log\ \cos2x\}{1+|y|}$ <br>
(iv) $z =e^x+ \log\ y+ pqr(s-t)$ <br>
(v) $T =\sin(a)\ cos(b) - |g-h|+\sqrt{ab}$ <br>
(vi) $z\frac{\alpha+\beta}{\sin\ x^o} + \frac{a^b+c^d}{a+b}$ <br>
(vii) $y = \sin\ \omega \pi\ \cos\frac{\omega\pi}{t}$ <br>

Ans : 
```
i. (a + b) / (c + d)
ii. (a * b) / (pow(c, 2) + d) * g
iii. sqrt(1 + x) * (log(cos(2 * x)) / (1 + fabs(y)))
iv. z = exp(x) + log(y) + p * q * r * (s - t);
v. T = sin(a) * cos(b) - fabs(g - h) + sqrt(a * b);
vi. z * (alpha + beta) / sin(x * M_PI / 180) + (pow(a, b) + pow(c, d)) / (a + b)
vii. y = sin(omega * M_PI) * cos((omega * M_PI) / t); 
```

6. Explain the program structure in C language.<br>

Ans : 
```c
<Header files>

<Global declaration of variables>

main()
{

  <Local declaration of variables>

  --------------

  <Statements>

  --------------

}

<Sub programs - function blocks>
```
1.The header files or preprocessor directives gives instructions to the compiler to include compiler options(#include),macro substitution(#define) to substitude a constant for an identifier and conditional(#ifdef) directives.<br>
2. The main statement block, function block and other blocks used in C program are enclosed in braces {}.<br>
3. Variables declared outside main() are called global variables, and they can be used in the main program block and sub program block.<br>
4. Variables declared inside main() are called local variables, and they are used only in the block in which they are declared.Sub programs/functions can also have local variables.<br>
5. Any C program has coding in the form of letters and symbols.Normally documentation to the program is made by adding remarks or comment lines enclosed  in /* and */ whenever necessary.<br>

7. Explain the different data types in C.<br>
Ans :<br>

i. `int` : *refers to interger. It can hold a signed or unsigned whole number within specific range.*
  
ii. `char` : *refers to characte. It can hold one letter/symbol. In fact, char in C language is associated with integers refers to a letter/symbol as per ASCII which has assigned integer value for all letters/symbol used in programming.*
  
iii. `float` : refers to floating point or real number. It can hold a real numeber like 3.174813 or 4.53e6 with six decimal digits in decimal or exponential form.,

iv. `double` : also refers to floating or real number. It can hold a real number in double precision. A double precision number uses 12 decimal digit like 3.42134421232 or 4.2324452423e12.


8. Discuss increment and decrement operators available on C and the rules associated with them.<br>
Ans : Increment operator(++) is used to increase the value of an integer or char variable by 1.Decrement operator(--) is used to reduce the value of an integer or char by 1.
      m++ and m-- are referring the post-fix increment and decrement operation, and ++m and --m are referrring the prefix increment and decrement operation.Post-fix increment first assign the value of the variable
      then increment it. Whereas, the prefix increment first increase the value and then assign the value of variable.

9. Explain arithmetic and logical operators in C with suitable examples.<br>

Ans : Arithmetic operators are used to perform arithmetic operations while assigning a value to a variable.<br>
      example : m += 10, this is evaluated as m = m + 10 , it increase the value of m then assigns the new value of m to m.<br>
      Logical operators are used to connect more relational operations to form a complex expression called logical expression.A value obtained by evaluating a logical expression is always logical, i.e either true or false.<br>
      example : (5 > 2) && (5<7) = True , this check the both condition if 5 is greater than 2 and 5 is less than 7 if both are true then the result is also true.<br>

10. Explain bitwise logical operators available in C. Discuss the order of evaluation.<br>

Ans : 
    1. Bitwise Left Shift(<<) : It is used to shift a bit position by inserting new bits at left side.<br>
    2. Bitwise Right Shift (>>) : It is used to shift a bit position by inserting new bits at right side.<br> 
    3. Bitwise AND (&) : It is used to compare a binary number and the result can be 1 only when both bits are 1.<br>
    4. Bitwise OR (|) : It is used to compare a binary number and the result is 1 when any of the bit is 1 result can be 0 only when both bits are 0.<br>
    5. Bitwise Inversion(~) : It is used to invert a binary number. The operator turns the 1 bit to 0 and 0 bit to 1.<br>
    6. Bitwise Exclusive OR (^) : It is used to compare a binary number.The result is 1 when both bits are different and 0 when the bits are same.<br>
    The order of evaluation : <br>
    1. Bitwise Left Shift<br>
    2. Bitwise Right Shift<br>
    3. Bitwise Inversion
    4. Bitwise AND
    5. Bitwsie OR
    6. Bitwise Exclusive OR

11. List the different types of operators in C. Discus the following with examples: (a) conditional operators (b) relational operators.<br>
# SHORT QUESTIONS 
1. C language has been developed by <ins>Dennis Ritchie</ins>.
2. Like decimal number system, octal and hexadecimal system can also be used in C language. (True/False) : `TRUE` 
3. An octal mumber is preceded by <ins>0</ins>and a hexadecimal number in preceded by <ins>0x</ins> 
4. An identifier/variable can begin with `_`(underscore). (True/False)  :  `TRUE`
5. Mention the basic data types used in C language. <br>
Ans : The basic data types used in C language are : <br>
    int, char, double, float etc.

6. A variable declared as `long int` occupies <ins>4</ins> bytes of memory.
7. If 'a' is an integer variable, then a=5/2 will return value <ins>2</ins>.
    8. Bitwise operators are for manipulation of <ins>data</ins> in bit level.
9. Define nibble and byte.<br> 
Ans : Nibble:
A nibble is a group of 4 bits (half of a byte). It can represent values from 0 to 15 in decimal (or 0000 to 1111 in binary).

Byte:
A byte is a group of 8 bits. It is the basic addressable unit of memory in most computer systems and can represent values from 0 to 255 in decimal (00000000 to 11111111 in binary).

11. Explain ternary operator. <br>

Ans : Ternary operator is used to check a condition and select a value depending on the value of the condition.
      The syntax of ternay operator is : <br>
      Variable = (condition)? value1 : value2;<br>
      when the condtion is evaluated, if the condition is `true`, the `value1` is assigned to the variable and if the condition is `false` the `value2` will be assigned to the variable.   

12. What is the purpose of type declaration in C?<br>
Ans : The purpose of type declaration in C is to define the type of data that a variable can hold

13. What are library functions? Mention any four library functions in C (functions available in math.h)?
14. What are the logical operators available in C? 
15. How does x++ differ from ++x? 
16. <ins>|</ins> is the operator which represents the bitwise OR operator. 
17. What is an identifier? 
18. A variable in C can be declared as float (real) if it is within the range _________ to ___________.
19. The relational operation that are commonly used in C are,__________,___________,_________,___________,___________,_________.
20. In C language a comment starts with the symbol _________ and ends with ___________.
21. Discuss the increment operator in C. 
22. Discuss the decrement operator in C.
23. What are the bit operators used in C.
24. Determine the value of the following logical expression for a=5, b=10, c=-6.
    (i) a == c ¦¦ b > a
    (ii) b > c && < 0 a > 0
25. Which of the following identifiers are invalid.
    (i) total
    (ii) average_value
    (iii) 6month
    (iv) cd 200
    (v) _sum
    (vi) rate$
26. For 9%4 the output is _________.
27. i += 1 can also be written as _____________.
28. __________ is the operator which represents bitwise exclusive OR.
29. How does the type `float` differ from `double` in C language? 
30. What is an operator? What is an operand? 
31. Explain with an example the usage of shorthand assignment operator. 
32. Mention the applications of C language. 
33. What do you mean by case-sensitive? Is C a case-sensitive language? 
34. ___________ data items are real data items that provide greater precision than is normally provided by the real data items.
35. Give the declaration for the string "COMPUTER" in C. 








 
