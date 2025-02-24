# Due Date: March 05, 2025, 11:59PM EST

# Lab 3: Hardware Modeling and Mapping Exploration
This lab aims to help you get a good understanding of hardware design space
exploration and mapspace exploration of DNN accelerator designs. Please watch
the released [video lectures](http://accelergy.mit.edu/tutorial.html) on
Accelergy and Timeloop to get a basic understanding of the tools that will be
used in this lab.

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