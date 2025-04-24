# CudaAtScaleIP

## Project Description

This project explores filtering and image processing using the CUDA NPP Library. It includes implementations for several image filters and allows users to process BMP or PGM image files. The project is designed to run in a Coursera Lab environment, providing a pre-configured CUDA setup.

Implemented Filters

The following filters are currently supported:

Canny Edge Detection (canny)

Sobel Edge Detection (sobel)

Gaussian Smoothing (gauss)

Sharpening (sharpen)

Features

Input Format: Supports BMP and PGM image files.

Output: Allows specifying an output file or directory for processed images.

Single Image Processing: Due to an NPP kernel execution issue, only one image can be processed per run.

Requirements

The project requires the Coursera Lab environment to execute. This environment provides a pre-configured CUDA setup, eliminating the need for additional configuration.

Project Structure

The project is based on the CUDA at Scale for the Enterprise Course Project Template.

Usage

Select an input image in BMP or PGM format.

Specify the desired filter from the implemented options.

Provide a filename or directory for the output file.

Known Limitations

Single Kernel Execution: The project currently supports processing only one image per run due to an issue with NPP kernel execution when reusing the same kernel.

## Code Organization

```bin/```
This folder should hold all binary/executable code that is built automatically or manually. Executable code should have use the .exe extension or programming language-specific extension.

```data/```
This folder should hold all example data in any format. If the original data is rather large or can be brought in via scripts, this can be left blank in the respository, so that it doesn't require major downloads when all that is desired is the code/structure.

```lib/```
Any libraries that are not installed via the Operating System-specific package manager should be placed here, so that it is easier for inclusion/linking.

```src/```
The source code should be placed here in a hierarchical fashion, as appropriate.

```README.md```
This file should hold the description of the project so that anyone cloning or deciding if they want to clone this repository can understand its purpose to help with their decision.

```INSTALL```
This file should hold the human-readable set of instructions for installing the code so that it can be executed. If possible it should be organized around different operating systems, so that it can be done by as many people as possible with different constraints.

```Makefile or CMAkeLists.txt or build.sh```
There should be some rudimentary scripts for building your project's code in an automatic fashion.

```run.sh```
An optional script used to run your executable code, either with or without command-line arguments.
