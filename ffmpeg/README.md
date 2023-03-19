# How to use/install ffmpeg using Docker

This Dockerfile provides a way to install `ffmpeg` on any system that has Docker installed.
Prerequisites

Docker must be installed on the host system.
Access to the internet to download the base Ubuntu image and `ffmpeg` package.

## Installation

To build the Docker image:

Clone the repository or download the Dockerfile.
Open a terminal and navigate to the directory containing the Dockerfile.
Run the following command to build the Docker image:

    docker build -t ffmpeg .

After the build process completes, run the following command to start a container:

bash

    docker run -it --rm ffmpeg -version

This command will print the version of `ffmpeg` installed in the container.

## Usage

After installing `ffmpeg`, you can use it to perform a variety of tasks such as converting video and audio files, resizing videos, and applying filters.

To use `ffmpeg` in a Docker container, simply run the docker run command and specify the desired `ffmpeg` command as an argument to the container. For example, to convert a video file to another format, run the following command:

bash

    docker run -it --rm -v /path/to/input:/input -v /path/to/output:/output ffmpeg -i /input/inputfile.mp4 /output/outputfile.avi

In this example, the -v option is used to mount two volumes (/path/to/input and /path/to/output) inside the container. The input file is located at /input/inputfile.mp4 and the output file will be saved as /output/outputfile.avi.

Note that you can modify the `ffmpeg` command to suit your specific needs.

## References

-   FFmpeg Documentation
-   Docker Documentation

