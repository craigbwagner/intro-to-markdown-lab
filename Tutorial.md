# Recursion in Programming
* *Recursion* occurs when a function calls itself directly or indirectly. This kind of function is known as a *recursive function*
    * A recursive function solves a problem by calling itself to solve subproblems of the original problem
    * In order to end the loop, a certain case, known as the *base case*, must be provided
* Recursion can reduce the length of code and makes code easier to read and write

## Using Recursion
**Algorithm Steps:**

1. Define a base case for which the solution is known
    * This serves as the stopping condition
    * Without a base case, the function will infinitely loop
2. Define a recursive case for which the function will recur
    * Consider how the problem can be solved in terms of smaller subproblems
    * Call the function again to solve those subproblems
3. Ensure the recursion terminates
    1. Make sure the recursion eventually reaches the base case
4. Combine the solutions to the subproblems to solve the original

***Example***
``` javascript
function factorialize(n) {
	if (n === 0) {  //base case
		return 1;
	} else {
		return n * factorialize(n - 1);  //recursive case
	}
}
```

For more information and to see examples, visit the [MDN docs](https://developer.mozilla.org/en-US/docs/Glossary/Recursion) or [Wikipedia](https://en.wikipedia.org/wiki/Recursion_(computer_science)) pages on recursion
