# infrared-SearchAndRescueDrone
This project aims to simulate how a search- and-rescue drone can detect survivors in low- visibility environments using infrared imaging.  By combining AI-based detection with drone- style footage, the system demonstrates how  technology can support faster, safer rescue operations.
PROJECT: Thermal Search & Rescue Drone Detection System
STUDENT: Harshita Gupta
COURSE: B.Tech. Computer Science & Design Engineering

-------------------------------------------------------------------------
PROJECT OVERVIEW
-------------------------------------------------------------------------
This project implements an automated human detection pipeline for search 
and rescue operations using thermal (infrared) drone footage. It utilizes 
Transfer Learning on the YOLOv8 architecture to identify human heat 
signatures in low-contrast environments.

-------------------------------------------------------------------------
CONTENTS
-------------------------------------------------------------------------
1. best.pt                             - The fine-tuned YOLOv8 model weights (The "Brain").
2. train_batch2                        - Training performance metrics (Precision/Recall).
3. Drone_infrared_detection            - Jupyter Source File
4. droneRawVid.mp4                     - Raw footage from Drone
5. droneinfrared.avi                   - The processed video with detection boxes.
6. requirements.txt                    - List of Python dependencies.

-------------------------------------------------------------------------
HOW TO RUN
-------------------------------------------------------------------------
The code is optimized to run on Google Colab (Free T4 GPU Tier).

1. Upload 'Thermal_Drone_Detection_Code.ipynb' to Google Colab.
2. Upload the raw video file to the Colab 'Files' directory.
3. Install dependencies by running the first cell (!pip install -r requirements.txt).
4. Run the 'Prediction/Inference' cell to generate the output video.

project demo: https://drive.google.com/drive/folders/1C3bZe5IubyjkM1LYkT8XDlm-8T7SG-zD?usp=sharing
-------------------------------------------------------------------------
TECHNICAL HIGHLIGHTS
-------------------------------------------------------------------------
- Custom Dataset: Curated and annotated thermal imagery 
- Optimization: Stream-based inference implemented to prevent RAM overflow 
  on limited hardware (O(1) memory complexity).
- Accuracy: Model achieved >80% precision on validation set.
