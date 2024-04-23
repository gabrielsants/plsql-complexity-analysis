# **Perform object complexity analysis**

This project is designed to perform complexity analysis on PL/SQL objects, such as procedures, functions, and packages. Below, you'll find an overview of what object complexity is, which keywords are relevant for evaluation, and how to calculate it within the context of this project.

![Badge](https://img.shields.io/github/license/gabrielsants/plsql-complexity-analysis)
![Badge](https://img.shields.io/github/forks/gabrielsants/plsql-complexity-analysis)
![Badge](https://img.shields.io/github/issues/gabrielsants/plsql-complexity-analysis)
![Badge](https://img.shields.io/github/stars/gabrielsants/plsql-complexity-analysis)
![Badge](https://img.shields.io/badge/Project%20Status-Building-yellow)


## **What is object complexity?**

Object complexity refers to the intricacy and difficulty of understanding and maintaining a given PL/SQL object, such as a procedure or function. It encompasses factors such as the number of lines of code, nesting levels, cyclomatic complexity, and the presence of complex SQL queries or logic structures.

## In PL/SQL, which keywords are candidates for evaluation?

1. **Control Flow Keywords:** Keywords such as IF, ELSE, ELSIF, CASE, LOOP, WHILE, and FOR contribute to control flow complexity due to their impact on program logic and branching.
2. **Exception Handling Keywords:** Keywords like EXCEPTION, RAISE, BEGIN, END, and DECLARE are important for evaluating how error handling is implemented within the object.
3. **SQL Keywords:** Keywords related to SQL operations, such as SELECT, INSERT, UPDATE, DELETE, MERGE, and FETCH, are crucial for assessing the complexity arising from database interactions.
4. **PL/SQL-specific Keywords:** These include keywords like DECLARE, BEGIN, END, FUNCTION, PROCEDURE, PACKAGE, RETURN, IS, AS, CURSOR, TYPE, RECORD, and ARRAY, which are fundamental to PL/SQL programming and contribute significantly to object complexity.

## How to calculate object complexity?

1. **Line Count:** Measure the number of lines of code within the object. More lines generally indicate higher complexity.
2. **Nesting Levels:** Count the levels of nesting for control flow structures like IF statements, loops, and subprograms. Deeper nesting levels imply increased complexity.
3. **Cyclomatic Complexity:** Calculate the cyclomatic complexity using a formula like McCabe's Cyclomatic Complexity, which considers the number of decision points and the overall structure of the code. Higher cyclomatic complexity values indicate greater complexity.
4. **SQL Complexity:** Evaluate the complexity of SQL queries within the object, considering factors such as the number of joins, subqueries, and conditions.
5. **Functional Complexity:** Assess the complexity of the object's functionality, including the number of parameters, the complexity of logic within functions or procedures, and the extent of error handling mechanisms.