+++
# Date this page was created.
date = 2018-11-10T00:00:00
layout = "project"

# Project title.
title = "Pipelined CPU implemented on FPGA"

# Project summary to display on homepage.
summary = """
 This is the curriculum design for our computer achitecture course.<br>
 I'm responsible for the ALU and pipeline design
 """
 
# image_preview = "MIPS_CPU/FPGA.png"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Programming","Hardware","CS"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# [header]
# image = "MIPS_CPU/FPGA.png"

+++

# Overview
Based on gate-level circuit design, we implemented a 32 bits CPU in Verilog. It contains the main parts of a fully
functional pipelined CPU. Then we embedded deep pipeline into the ALU. <br>
We ran 100 8-point
FFT algorithm on it, And tested the project on FPGA (We used Basys, which is specifically designed for Vivado Design Suite). It is proved to be efficient 
and reliable. <br>

The main work for the project is as follows: <br>
1. The eight-staged pipelined CPU design and implementation, including the control part as well as data path. <br>
2. High efficiency assembly language of FFT. <br>
3. Hazard detection and the test of FFT on the simulated CPU.

# Main Module Design
## ALU (mainly on Multiplier)
We were required to implement gate-level Arithmetic Logical Unit (unlike behavior-level 
ALU, we were requested to implement the detail of the gates). When implementing it, we firstly designed
a simple unsigned multiplier based on the image below. 
![Multiplier Unit.png](https://upload-images.jianshu.io/upload_images/20282999-bf3f4190652a0dd1.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
And applied the operation of adding, shifting as well as choosing to implement the function of multiplying
by bits. Here are 32-bit analytical circuit and the waveform of simulation.
![32-bit multiplier.png](https://upload-images.jianshu.io/upload_images/20282999-5da882701048c11b.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![waveform of multiplier.png](https://upload-images.jianshu.io/upload_images/20282999-31c1ba0a8d0fa896.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
## Datapath and Control
### Control
### Pipeline and Datapath
## Test
### FFT
### Test on FPGA

# Final Words
## Future Work
## Acknowledgement
It's really a great project, thank you for Prof. Jianhao Hu, Prof. Shang Ma and Associate Professor Jienan Chen, they provided us with amazing materials.
And it was great time work with Zhongyao Cao and Sufang Yang, they both are young researchers and partners.

![Digital Circuit](https://upload-images.jianshu.io/upload_images/20282999-98c9f5b101a0f623.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
