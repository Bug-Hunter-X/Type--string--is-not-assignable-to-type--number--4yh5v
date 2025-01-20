# Type 'string' is not assignable to type 'number'

This repo demonstrates a common TypeScript error: assigning a string to a variable that is type-annotated as a number.

## Description
The TypeScript compiler correctly flags this as an error because it enforces type safety.  Attempting to perform mathematical operations on a string will result in unexpected behavior at runtime. 

## How to reproduce

1. Clone this repository.
2. Open `bug.ts`.
3. Attempt to compile and run the code using the TypeScript compiler (`tsc bug.ts` and then `node bug.js`).

You will encounter a compilation error.

## Solution
See `bugSolution.ts` for a corrected version of the code that handles type safety.