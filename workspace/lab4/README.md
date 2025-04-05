# Due date: Friday, March 14th, 2025, 11:59 PM

# Lab 4: Sparse Matrix Multiplication and Hardware Optimization

In this lab, we will explore opportunities for optimizing sparse matrix multiplication in hardware. We'll examine different optimization techniques like gating and skipping, and understand their impact on latency and energy efficiency. The lab will cover:

- Dense vs sparse matrix multiplication
- Optimization opportunities in sparse computations
- Hardware techniques for handling sparsity
- Energy and latency trade-offs

## Part 1: Sparse Optimization Opportunities in Matrix Multiplication

In this section, we will:
1. Review dense matrix multiplication as a baseline
2. Explore how sparsity creates opportunities for optimization
3. Analyze two key optimization techniques: gating and skipping
4. Calculate the potential savings in computation and energy

Answer questions 1.0-1.7

## Part 2: Saving Energy with Gating

In this section, we will explore how gating can be used with sparse matrix multiplication. We will experiment with sparse architectures using Sparseloop (an extension of Timeloop to support sparse architectures).

Answer question 2.1

## Part 3: Increasing Throughput and Energy Efficiency with Skipping And Compression

In this section, we will analyze how skipping affects sparse matrix multiplication. For this part, we will compress both input operands and perform skipping.

Answer questions 3.1-3.3

## Part 4: The Effect of Sparsity on Compressed Tensor Buffer Space Usage
In this section, we will see how different levels of sparsity affect buffer space usage when using compressed formats.

Answer questions 4.1 and 4.2

## Part 5: Breaking Assumptions

For the previous sections, you were asked to assume that *all tensors are independently distributed*. While this statement tends to hold for DNNs, it is not generally true for sparse matrix multiplication. Here, we will explore how different density distributions can change the number of effectual operations and how different input densities affect the output. 

Answer questions 5.1-5.3

## Part 6: Designing a Sparsity-Aware Matrix Multiplication System

This part is in lab4_design.ipynb

For this section, you are given a template sparse matrix multiplication accelerator. Your job is to figure out the best dataflow to use with on 5 sparse matrix multiplication workloads given three different compression formats - you will be optimizing to minimize energy and cycles. 

Fill in 6.1 and 6.2, then answer the questions in 6.3-6.6

Grading Scheme:
- Parts 1-5, 6.3-6.6: 50% in total
- Part 6.1: 25%
- Part 6.2: 25%

## Additional Resources

For more information on the tools available for handling sparsity in Timeloop, please review the [Sparseloop paper](https://sparseloop.mit.edu/documents/2022-micro-sparseloop.pdf), [Sparseloop tutorial video](http://accelergy.mit.edu/sparse_tutorial.html), and [Sparseloop MICRO artifact](https://github.com/Accelergy-Project/micro22-sparseloop-artifact). The MICRO artifact in particular may be helpful for final projects relating to sparsity. 