# MandelbrotParallelization
Premanshu Patel, Himanshu Patel, and Yongxu Wang
This repo include our code and output

This is our Mandelbrot set Parallelization where we use OpenMP, OpenACC on multicore and GPU
The purpose of the project is to find the which parallelization method was the fastest

Hardware:
For the hardware we used the supercomputer Bridges2 to compile and run the code, and also we used the NVC compiler aswell. The way we tested which parallelization method was the best was by running the code with different number of cores (only for OpenMp and OpenACC Multicore) and measuring the time for each run.

For OpenACC GPU we used the Bridges2 Tesla GPUs

Conclusion:
In conclusion we saw that OpenMP was the fastest out of the other parallelization methods, it was also about twice as fast OpenACC Multicore

Also we ran into an issue with compile the code for the GPU where it didn't allow us to use the code that created the image of the Mandelbrot Set, so we had to comment that code, and that is why it was drastically faster then the other parallelization methods since it was not creating the image.
