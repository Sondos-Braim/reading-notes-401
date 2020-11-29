# Read 2


## In Tests We Trust — TDD with Python

-Test-driven development (TDD) is a software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases. This is opposed to software being developed first and test cases created later.

-We need to walk through the process using baby-steps.

-The greatest advantage about TDD is to craft the software design first

-Your code will be more reliable: after a change you can run your tests and be in peace

-Beginning may be hard — and that’s fine. You just need to practice!

## Recursion

What is Recursion? 

-The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function. Using recursive algorithm, certain problems can be solved quite easily.

- the function itself is being called inside the function, so this phenomenon is named as recursion and the function containing recursion is called recursive function, at the end this is a great tool in the hand of the programmers to code some problems in a lot easier and efficient way.

-In the recursive program, the solution to the base case is provided and the solution of the bigger problem is expressed in terms of smaller problems.

-The idea is to represent a problem in terms of one or more smaller problems, and add one or more base conditions that stop the recursion.

-If the base case is not reached or not defined, then the stack overflow problem may arise.

-A function fun is called direct recursive if it calls the same function. A function is called indirect recursive if it calls another function directly or indirectly.

-A recursive function is tail recursive when recursive call is the last thing executed by the function.

-When any function is called from main(), the memory is allocated to it on the stack. A recursive function calls itself, the memory for a called function is allocated on top of memory allocated to calling function and different copy of local variables is created for each function call. When the base case is reached, the function returns its value to the function by whom it is called and memory is de-allocated and the process continues.
