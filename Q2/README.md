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

/assets/images/Screenshot from 2022-11-21 17-33-23.png