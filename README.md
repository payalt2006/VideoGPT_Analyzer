# Video Analyzer using Machine Learning
# Video Analyzer and Chatbot


This project aims to automatically analyze videos and generate summaries using a combination of advanced techniques. Additionally, it creates a chatbot that can answer questions about the video content. The system employs methods such as superframe cuts, motion scores, and uniqueness scores to extract key information from videos and generate concise summaries. The chatbot is trained using these keyframes to provide relevant responses to user queries about the video.

## Purpose

The purpose of this project is to create a system that can automatically analyze videos, generate summaries, and provide interactive responses to questions about the video content. This system can be applied in various domains, such as educational video summarization, accessibility for individuals with disabilities, or creating engaging video experiences.



## Implementation

The project follows a series of steps to analyze videos and train the chatbot:

1. Video Conversion: The video is first converted into individual frames to facilitate further analysis.

2. Scoring Mechanisms: Each frame is evaluated using scoring mechanisms such as superframe cuts, motion scores, and uniqueness scores. These mechanisms help identify frames with significant content, motion, and uniqueness.

3. Keyframe Selection: Frames with the highest scores are selected as keyframes, representing important moments in the video. These keyframes serve as a summary of the video content.

4. Additional Models: Additionaly it has two other methods one for object detection using yolo8x and other for motion detection using model trained using ucf 101.

5. Captions : The detections from all the model are appended in the captions.txt file.

6. Chatbot Training: The keyframes from the captions.txt are used to train a chatbot model. The chatbot learns to generate descriptive text based on the keyframes, enabling it to answer questions and provide information about the video content.

## Getting Started

To get started with this project, follow these steps:

1. Clone the repository to your local machine.
2. Navigate to the project directory.
3. Install the required dependencies by running the following command:pip install -r requirements.txt
4. Save your Video in video folder and rename it as NYTravel.mp4 as the full code uses it only for the input file additionally you can change the video path also from the code but it would be cumbersome. So only rename it as NYTravel.mp4 only.
5. Run the following jupyter notebooks and to generate keyframes and train the chatbot:
                     GetKeyFrames-1
                     inference-2
                     chatbot-3

## FULL WORKING CODES WITH MODELS DRIVE LINK: https://drive.google.com/drive/folders/1QuCklGGkYjp1kkgw47df8RaxxzGyhZXK?usp=sharing

## References
I took the reference of below cited papers:
Presented at [2022 Asian Conference on Innovation in Technology (ASIANCON)](https://ieeexplore.ieee.org/xpl/conhome/9908521/proceeding)

DOI: [10.1109/ASIANCON55314.2022.9909008](https://doi.org/10.1109/ASIANCON55314.2022.9909008)
