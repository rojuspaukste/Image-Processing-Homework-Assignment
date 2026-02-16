# Image-Processing-Homework-Assignment

## Introduction
This repository stores everything related to the Homework assignment of Image Processing course for AI Engineering Masters in VGTU:
1. Source code
2. Input data
3. Output data & key artifacts
4. Presentation
5. Peer review

## About this assignment
The purpose of this assignment was to create an exercise counter. It is expected to take a video of a person doing an exercise as input and output an annotated video with a counter incrementing for each rep.

***(gif of output)***

## How it works
The source code can be found in the following folder ***(Exercise Counter/src)***. It is written as a python notebook file for better readability and easier visualization of the outputs.

To put it simply, the code itself works by taking a video, processing each of its frames and drawing landmarks (points of interest, in this case joints). It then calculates the angle between joints during each frame and logs it into a dataset. We count reps by swapping states when the angle between the joints changes over a certain threshold. To annotate the video we find those key frames when the state swap happens and increment the counter once we return to the starting state. 

***(screenshot of rep plot)***

A more detailed explanation of each step can be found inside the comments of the source code (I hope its understandable :D)

## How to use it
As mentioned, all the input and output data is already in place, so there is no need to download anything else, just clone this repository. 

The source code is all located in a single file so all you have to do is run it on your local machine.

Additionally, the section called "Paths and basic config" allows us to swap over which example video is processed. 

***(screenshot of paths and configs)***

So far we only account for one exercise, that being squats. However, with a little bit of work, this can easily be extended to other exercises such as jumping jacks, pushups, situps bycep curls or any other exercise that revolves around us changing angles over specific body parts :)



