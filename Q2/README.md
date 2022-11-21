# Solution for Q2 (4.24)

## Implementation
- Two different programs are written for the implementation of this problem.
- One is a serial approach that is carried out on a single thread.
- The other is a parallel approach that makes use of the multi-threading idea to implement the different functionalities, such as generating random      coordinates, checking whether they lie within the circle, and finally the estimation of pi on different threads.
- The comparision of the two approaches is given in the inferences.
- 900000000 random points were plotted in order to make the estimation.

## Running the Programs
### single.c
- gcc single.c -o serial.o
- ./serial.o

Output

![Screenshot from 2022-11-21 17-33-23](https://user-images.githubusercontent.com/79468881/202982289-a1a2a02e-cba1-4cac-82f3-4f47b7906c30.png)

### parallel.c
- gcc parallel.c -o parallel.o
- ./parallel.o

Output

 ![file:///home/palgun/Pictures/Screenshot%20from%202022-11-21%2017-34-32.png](Images/Screenshot%20from%202022-11-21%2017-34-32.png)

## Conclusions
- The serial approach takes 23.194199s.
- The parallel approach takes 8.574160s.
- Hence we can see that the serial takes almost 2.7 times longer.

**Thus we can conclude that by taking a multi-threaded approah helps in faster computation**

## References
- [https://github.com/SeanStaz/monteCarloMethod.c/blob/master/A3.c](https://github.com/SeanStaz/monteCarloMethod.c/blob/master/A3.c)
- [https://github.com/ilias1111/parallel-monte-carlo-pi](https://github.com/ilias1111/parallel-monte-carlo-pi)

