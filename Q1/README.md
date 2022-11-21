# Solution to Q1 (3.21)

## Implementation
- An approach for the solution to the Collatz Conjecture is given here.
- First the parent process invokes the child process through the fork() command, since both will carry copies of the data, it is necessary for the child to print the output values.
- The input is taken by the parent process.
- The parent invokes the wait() call.
- ie. Only after the child process finishes printing the values, only then the parent can complete execution.

## Running the Code
- gcc collatz.c -o collatz.o
- ./collatz.o

Output

![Screenshot from 2022-11-21 18-08-13](https://user-images.githubusercontent.com/79468881/202988052-e6e08438-8b28-4ec7-96d4-4eba69d34593.png)

## Inferences
- Therefore it can be observed that both parent and child create different copies of data.
- When the parent calls the fork() operation it waits till child completes execution.
- Only then the parent resumes, in this case proceeds to terminate.

## References
- [https://github.com/SeanStaz/theCollatzConjecture.c/blob/master/hailstone.c](https://github.com/SeanStaz/theCollatzConjecture.c/blob/master/hailstone.c)
- [https://github.com/Samith-hegde/CollatzConjecture](https://github.com/Samith-hegde/CollatzConjecture)
