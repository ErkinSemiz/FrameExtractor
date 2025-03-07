# Frame Extractor for Drone Recorded Videos

![image](https://github.com/user-attachments/assets/acb12ffa-2bdd-4480-9660-1a6ed4f954a8)

**Creator:** Erkin Semiz  

[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-310/)
[![OpenCV 4.5.5](https://img.shields.io/badge/OpenCV-4.5.5-red.svg)](https://pypi.org/project/opencv-python/)
[![Tkinter](https://img.shields.io/badge/Tkinter-8.6-red.svg)](https://docs.python.org/3/library/tkinter.html)

**Environment File:** `python310MLfinal.yaml`  
**Requirements File:** `requirements.txt`  

---

## **Project Overview**
This project provides a tool for extracting frames from drone-recorded videos. The extracted frames can be used for further processing, such as training machine learning models for various applications.

---

## **Project Folder Structure**
PROJECT/ 
├── data/ 
    ├── frames/ # Extracted frames from videos │ 
    ├── videos/ # Input video files (grayscale and color) │ 
        ├── example_gray.mp4 │ 
        ├── example_color.mp4 
├── scripts/  
    ├── FrameExtractor.py # Script to extract frames from videos │ 
    ├── FrameExtractorUI.py # UI for frame extraction │ 
├── python310MLfinal.yaml # Anaconda environment file 
├── requirements.txt # Python dependencies 
└── README.md # Project documentation

---

## **Project Workflow**
The project is divided into three major phases:

### **1. Frame Generation**
The first phase involves generating frames from input videos. You can extract frames using the script `FrameExtractor.py` or its corresponding UI version, `FrameExtractorUI.py`.

**Steps**:
1. Place input videos in the `data/videos/` directory.
2. Specify the input video path and save directory in the script or use the UI to select them interactively.
3. Run the script to extract frames into `data/frames/`.

**Example:**
python scripts/FrameExtractor.py

Output:
Frames are saved as frame_0000.jpg, frame_0001.jpg, etc., in the specified directory.

### **Setup Instructions**
1. Prerequisites
    Python 3.10
    Anaconda (recommended)
2. Setting Up the Environment
Using Anaconda:

    conda env create -f python310MLfinal.yaml
    conda activate python310MLfinal

Using requirements.txt:

    pip install -r requirements.txt

### **Scripts Overview**
FrameExtractor.py
    Extracts frames from input videos and saves them as image files.
    Hardcoded paths for video and save directory can be replaced with dynamic user input through FrameExtractorUI.py.

### **Key Features**
    Automated Frame Extraction: Extract frames from videos for dataset creation.
    Interactive UIs: Easy-to-use interfaces for frame extraction and fire detection.
