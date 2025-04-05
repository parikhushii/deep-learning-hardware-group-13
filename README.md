# Project 6: Investigating the Impact of Sparsity in Operands and Results

# Lab 4: Sparse Matrix Multiplication and Hardware Optimization
This lab aims to help you get a good understanding of opportunities for optimizing sparse matrix multiplication in hardware accelerators. For detailed instructions, please read [./workspace/lab4/README.md](./workspace/lab4/README.md). 

## Using Docker

Please pull the docker first to update the container, and then start with `docker-compose up`. 
```
cd <your-git-repo-for-lab4>
export DOCKER_ARCH=<amd64 or arm64>
docker-compose pull
docker-compose up
```
After finishing the lab, please commit all changes and push back to this repository.


In this lab, we will explore how sparsity (zero values) can be leveraged to
reduce the memory footprint and number of operations executed in tensor
operations.

## Using Docker

Please start the Docker and the Jupyter server like in Lab 0. Please pull
the docker first and then start with `docker-compose up`.

```
cd <your-repository-directory>
export DOCKER_ARCH=amd64

# If you are using arm CPU (Apple M1/M2), 
# export DOCKER_ARCH=arm64 

docker-compose pull
docker-compose up

# Complete the lab then run the following from within the docker container
# make submit
```

## Submission
After finishing all of the provided notebooks, please run `make submit` to
submit your code. Check your submission on the GitHub website and ensure that
all notebooks have all cells run and all outputs visible. Additionally, ensure
that the `answers.yaml` file in the website matches the answers you have in your
notebooks. If either the notebooks or the `answers.yaml` file are not up to
date, you may lose points or receive a zero for the assignment.

FAILURE TO FOLLOW THESE INSTRUCTIONS WILL RESULT IN YOU RECEIVING A ZERO FOR THE
ASSIGNMENT.
