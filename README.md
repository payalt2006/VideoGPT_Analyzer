# VideoGPT Analyzer

### AI-Powered Video Analysis, Summarization & Chatbot

## Overview

**VideoGPT Analyzer** is an intelligent video understanding system that automatically analyzes video content, extracts meaningful insights, generates concise summaries, and enables interactive question answering through an AI-powered chatbot.

The project combines computer vision, motion analysis, object detection, and natural language processing to transform raw videos into searchable and conversational knowledge.

## Features

* 🎥 Automatic video frame extraction
* ✂️ Keyframe detection using intelligent scoring mechanisms
* 🏃 Motion analysis and activity recognition
* 🎯 Object detection using YOLOv8x
* 📝 Automated caption generation
* 🤖 Video-aware chatbot for question answering
* 📄 Video summarization using keyframe analysis

---

## Purpose

The purpose of this project is to build an intelligent system capable of:

* Automatically understanding video content
* Generating concise summaries
* Detecting objects and activities
* Enabling conversational interaction through a chatbot

This system can be applied in areas such as:

* Educational video summarization
* Accessibility support
* Surveillance and monitoring
* Smart video search and indexing
* Interactive video experiences

---

## Project Pipeline

The project processes videos through the following stages:

### 1. Video Frame Extraction

The input video is converted into individual frames for detailed analysis and processing.

### 2. Frame Scoring & Analysis

Each frame is evaluated using multiple scoring techniques:

* **Superframe Cuts** – Detects significant scene transitions
* **Motion Scores** – Measures movement and dynamic activity
* **Uniqueness Scores** – Identifies visually distinctive frames

These scoring methods help identify important visual moments within the video.

### 3. Keyframe Selection

Frames receiving the highest combined scores are selected as **keyframes**, representing the most informative content and generating a compact summary of the video.

### 4. Additional Detection Models

The system integrates two advanced models:

### Object Detection

* **YOLOv8x** is used to detect and localize objects in video frames.

### Motion Recognition

* A model trained on the **UCF101 dataset** is used for motion and human activity recognition.

### 5. Caption Generation

Outputs from all models are combined and stored in:

```text
captions.txt
```

This file acts as a textual representation of the video content.

### 6. Chatbot Training & Question Answering

The chatbot is trained using the generated captions and extracted keyframe information.

The chatbot can:

* Answer questions about video content
* Describe scenes and detected activities
* Provide contextual information from analyzed videos

---

## Tech Stack

* Python
* OpenCV
* YOLOv8x
* UCF101 Motion Recognition Model
* Jupyter Notebook
* NLP-based Chatbot
* Machine Learning & Computer Vision

---

## Getting Started

Follow these steps to run the project locally.

### 1. Clone Repository

```bash
git clone <repository-link>
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Prepare Input Video

Save your video inside the **video/** folder and rename it as:

```text
NYTravel.mp4
```

The current implementation uses this filename as the default input.

### 4. Run the Notebooks

Execute the following notebooks in order:

### GetKeyFrames-1

Generates keyframes from the video.

### inference-2

Runs detection models and caption generation.

### chatbot-3

Trains and launches the chatbot.

---

## Research Reference

This project takes inspiration from the following research paper:

**2022 Asian Conference on Innovation in Technology (ASIANCON)**

DOI:

10.1109/ASIANCON55314.2022.9909008

---

## Future Improvements

Potential future enhancements include:

* Real-time video summarization
* Speech-to-text integration
* RAG-based conversational retrieval
* Multi-video understanding
* Cloud deployment and APIs
* Multilingual chatbot support

---

## Author

Developed as a Machine Learning and Computer Vision project for intelligent video understanding and conversational AI.
