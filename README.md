# Infinite Loop in TypeScript `for` Loop

This repository demonstrates a common error in TypeScript: an infinite loop caused by using a negative number as the upper bound in a `for` loop.

## Bug Description
The `printNumbers` function intends to print numbers from 1 to `n`. However, when `n` is negative, the loop condition `i <= n` is always true, resulting in an infinite loop.

## Solution
The solution involves adding a check to ensure that `n` is non-negative before starting the loop. If `n` is negative, the loop is skipped, and a message can be printed if needed.

## How to Reproduce
1. Clone the repository.
2. Open `bug.ts`.
3. Run the code using a TypeScript compiler (e.g., `tsc bug.ts`) and then run the compiled Javascript file.
4. Observe the infinite loop when calling `printNumbers` with a negative number.
5. Open `bugSolution.ts`. 
6. Run the code using a TypeScript compiler (e.g., `tsc bugSolution.ts`) and then run the compiled Javascript file.
7. Observe that the infinite loop is avoided.

## License
MIT