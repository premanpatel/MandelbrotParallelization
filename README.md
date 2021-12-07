# MandelbrotParallelization
Premanshu Patel, Himanshu Patel, and Yongxu Wang
This repo includes our Mandelbrot Parallelization code and output

This is our Mandelbrot set Parallelization where we use OpenMP, OpenACC on multicore and OpenACC on GPU.
The purpose of the project is to find the which parallelization method was the fastest.

Hardware:
For the hardware we used the supercomputer Bridges2 to compile and run the code. We also used the NVIDIA HPC SDK (NVC) compiler. The way we tested which parallelization method was the best was by running the code with different number of cores (only for OpenMp and OpenACC Multicore) and measuring the time for each run.

For OpenACC GPU we used the Bridges2 Tesla GPUs.

Conclusion:
In conclusion we saw that OpenMP parallelization was faster than OpenACC parallelization, and OpenMP Multicore was about twice as fast as OpenACC Multicore.
OpenACC on GPU was the fastest runtime. 

Also we ran into an issue with compiling the code for the GPU where it didn't allow us to use the code that colored the image of the Mandelbrot Set, so we had to comment that code for it to compile. 
