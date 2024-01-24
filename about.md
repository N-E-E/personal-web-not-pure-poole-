---
layout: page
title: About Me
---


Hi, welcome to my personal website. I am a 3th year undergraduate student from Huazhong University of Science and Technology(HUST) majoring in Computer Science. I am passionate about computer architecture, including High Performance System, MLSys, and Next Generation Archs(CPUs, Compilers, In-Memory Computing and so on).

My CV is available [here](https://github.com/N-E-E/personal-web/raw/master/resource/CV.pdf). If it's not available, try [here](https://gitee.com/N_E_E/personal-web-resource/raw/master/CV.pdf)

## Research Experience
### 10/2022-11/2022: 
#### Scheduling of Data Retrieval Tasks in Tape Cloud Storage Systems(HUAWEI Coding Challenge)
- **[Code](https://github.com/N-E-E/2022-massive-storage-challenge)**
- A short time research experience, mentored by Prof. You Zhou
- In this research, the team and I solve a Data Retrieval Task and aim to minimize the tasks-waiting time under some limitations. What I did in this project is to discuss with team members, and do coding jobs to verify strategies.


### 01/2023-present:
#### Heterogeneous Graph Processing System with GPUs/FPGAs
- Under the supervision of Prof. Long Zheng
- In this project, what I mainly did is to get started in computer architecture and graph processing system. I spent some time learning CUDA programming and Verilog HDL(and a little xilinx hls) so that I can read source code of some papers. I think it is important skills for verifying my research ideas in computer arch.


#### Vision Transformer Acceleration under graph processing perspective
- **[Slide](https://github.com/N-E-E/personal-web/raw/master/resource/research3-slide.pptx)**(If not available, try [here](https://gitee.com/N_E_E/personal-web-resource/raw/master/research3-slide.pptx))
- With the assistance of Ph.D.graduate Yu Huang, under the supervision of Prof.Zheng Long
- It's a challenging experience for me but I enjoy and benefit a lot in the experience!
- In the beginning, I read some papers in LLM system optimization and acceleration, especially the acceleration techniques in attention mechanism.(sparsity, checkpoint, quantization, pruning and so on)
- Discussing with Ph.D.graduate Yu Huang. Searching and reading papers in transformer(mainly in attention mechanism) optimization with Graph methods. The key target is to solve the memory bound problem(increase FLOPS/BytesAccess). Inspired by order invariance of transformer and the similaration between graph and image, we propose "Img2Graph" and "Reorder" operations. An image can be transform to a graph, and then a "Reorder Operation" can be used to reorder the image patches from a graph, making similar patches stay together after the flatten operation in ViT. That is simple to make use of differentiated sparsity/quantization in matrix multiplication in the following progress.
- Do some experiments to verify ideas, and discuss with Mr.Huang.

## other projects
[A Five-Stage Pipeline Risc-V CPU](./_posts/2023-10-10-Riscv-CPU.md)

[A Compiler Frontend of C-like Language](./_posts/2022-10-12-my-simple-compiler.md)

[Android App for AI Drawing Online with Stable Diffusion(Software Engineering Course Project)](https://github.com/N-E-E/AI-Art-Mobile)

**For more projects, welcome to visit [my github](https://github.com/N-E-E)**


## Research Interests
- High Performance System
    - Heterogeneous Computing(GPUs, FPGAs)
    - Graph Processing System
- MLSys
    - Optimization and Acceleration Techniques
- Next Generation Archs
    - CPUs
    - In-/Near-Memory Computing
    - Compilers

## Main Skills
- C++/Python
- Engeneering Skills: Git/Make/CMake, modern C++ & design patterns, basic linux knowledge
- Pytorch
- CUDA programming
- Verilog HDL.
- Xilix HLS(a little)
