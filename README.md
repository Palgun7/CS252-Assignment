# CS252-Assignment
This assignment consists of two easy level questions adopted from the 10th edition of Opersting System Concepts.

[Q1. (3.21)](https://github.com/Palgun7/CS252-Assignment/tree/main/Q1)

The Collatz conjecture concerns what happens when we take any positive integer n and apply the following algorithm:

<img width="246" alt="Q" src="https://user-images.githubusercontent.com/79468881/202985769-c9c55359-a84d-41de-af9a-59eff1e9682c.png">

The conjecture states that when this algorithm is continually applied, all positive integers will eventually reach 1. For example, if n = 35, the sequence is 35, 106, 53, 160, 80, 40, 20, 10, 5, 16, 8, 4, 2, 1 Write a C program using the fork() system call that generates this sequence in the child process. The starting number will be provided from the command line. For example, if 8 is passed as a parameter on the command line, the child process will output 8, 4, 2, 1. Because the parent and child processes have their own copies of the data, it will be necessary for the child to output the sequence. Have the parent invoke the wait() call to wait for the child process to complete before exiting the program. Perform necessary error checking to ensure that a positive integer is passed on the command line.


[Q2. (4.24)](https://github.com/Palgun7/CS252-Assignment/tree/main/Q2)

An interesting way of calculating π is to use a technique known as Monte Carlo, which involves randomization. This technique works as follows: Suppose you have a circle inscribed within a square, as shown in Figure 4.25. (Assume that the radius of this circle is 1.)

• First, generate a series of random points as simple (x, y) coordinates. These points must fall within the Cartesian coordinates that bound the square. Of the total number of random points that are generated, some will occur within the circle.

• Next, estimate π by performing the following calculation:

π = 4× (number of points in circle) / (total number of points)

Write a multithreaded version of this algorithm that creates a separate thread to generate a number of random points. The thread will count the number of points that occur within the circle and store that result in a global variable. When this thread has exited, the parent thread will calculate and output the estimated value of π.

It is worth experimenting with the number of random points generated. As a general rule, the greater the number of points, the closer the approximation to π.

In the source-code download for this text, you will find a sample program that provides a technique for generating random numbers, as well as determining if the random (x, y) point occurs within the circle.





