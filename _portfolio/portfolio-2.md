---
title: "Variable Sized-Batch General Multiplication (Variable GEMM)"
excerpt: "
This repo improves Mixture-of-Experts (MoE) models by addressing load-imbalance during dynamic routing, enhancing inference performance on hardware 
accelerators. It integrates CuBLAS and CuSparse, optimizing batched GEMM tasks for variable-sized inputs, resulting in significant efficiency gains 
across different model sizes.<br/><img src='/images/VariableGEMM.png'>"
collection: portfolio
---

This repo delves into enhancing the inference performance of Mixture-of-Experts (MoE) models, a technique leveraging sparsity to achieve high 
capacities with moderate computational costs. We address the challenge of load-imbalanced computations during dynamic routing within MoE layers, 
which hampers real-world applications on hardware accelerators like GPUs and TPUs. We integrate existing libraries such as CuBLAS and CuSparse to 
augment our implementation. Our design includes a MoE layer with 64 experts, each processing variable-sized batches of inputs. We utilize CuBLAS's 
cublasSGemmGroupedBatched function for batched GEMM tasks with variable-sized entries, transforming inputs into column-major format and segregating
them into uniform-sized groups. This allows us to quantify the benefits of batching non-uniform GEMM operations against a baseline implementation. 
We evaluate our approach across three model sizes with varying numbers of experts and observe superior performance of variable-sized batching over 
the baseline, confirming the efficiency gains. Additionally, we note that increasing batch size leads to reduced computation time due to enhanced 
parallelization.
[PPT](https://docs.google.com/presentation/d/1zngkSWLxD7omhyueg6ARBHEXD4qJyhn06vY7VSojBbk/edit#slide=id.gc6f90357f_0_0)[Code](https://github.com/anirudh28/VariableGEMM)
