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

![annotated_video-ezgif com-video-to-gif-converter (2)](https://github.com/user-attachments/assets/05329912-3f29-4d22-b8c6-c654d164b402)

## How it works
The source code can be found in the following folder ***(Exercise Counter/src)***. It is written as a python notebook file for better readability and easier visualization of the outputs.

To put it simply, the code itself works by taking a video, processing each of its frames and drawing landmarks (points of interest, in this case joints). It then calculates the angle between joints during each frame and logs it into a dataset. We count reps by swapping states when the angle between the joints changes over a certain threshold. To annotate the video we find those key frames when the state swap happens and increment the counter once we return to the starting state. 

<img width="1190" height="390" alt="image" src="https://github.com/user-attachments/assets/03cb9c7e-1852-459f-a829-3c26f1a34e1d" />

A more detailed explanation of each step can be found inside the comments of the source code (I hope its understandable :D)

## How to use it
As mentioned, all the input and output data is already in place, so there is no need to download anything else, just clone this repository. 

The source code is all located in a single file so all you have to do is run it on your local machine.

Additionally, the section called "Paths and basic config" allows us to swap over which example video is processed. 

<img width="888" height="370" alt="image" src="https://github.com/user-attachments/assets/5b82041f-e58d-4b92-91ff-98103a88154c" />

So far we only account for one exercise, that being squats. However, with a little bit of work, this can easily be extended to other exercises such as jumping jacks, pushups, situps bycep curls or any other exercise that revolves around us changing angles over specific body parts :)

## For peer review team

So far the repo contains 3 squat examples I downloaded from online. If you would like to, you can replicate the same folder structure and include more of your own videos. The only requirements is that the video should preferably contain the whole body of a person doing squats and that it is filmed from the side view :)



