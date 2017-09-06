# Visual Recognition Environment Setup and Assignments

## Requirements
* Nvidia GPU Drivers (For employing GPU in ML)
* [docker](http://www.docker.com)
* [nvidia-docker](http://www.github.com/NVIDIA/nvidia-docker)

## Local Setup
1. Run `docker build -t <image_name> <Dockerfile location>` or `docker pull shivnshu/pytorchwithcuda`
2. Run `nvidia-docker run -v <folder_location>:/root/Project -p 8888:8888 --rm -ti --ipc=host <image_name>`
3. Run `jupyter notebook` in container and access web interface on host machine on url http://localhost:8888 (default password: shivnshu)
