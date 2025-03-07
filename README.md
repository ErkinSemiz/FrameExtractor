# Frame Extractor for Drone Recorded Videos

**Creator:** Erkin Semiz  
**Python Version:** Python 3.10 (Anaconda Environment)  
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