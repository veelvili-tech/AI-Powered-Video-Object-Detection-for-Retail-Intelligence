# AI-Powered-Video-Object-Detection-for-Retail-Intelligence
This project demonstrates a computer vision object detection pipeline built using a pretrained YOLOv8 model.
A short personal demo video (self-recorded) is used to validate the end-to-end pipeline, focusing on model inference, video processing, and deployment readiness rather than dataset collection.

# Project Background
Retail and physical-space businesses increasingly rely on video analytics to improve operations and customer experience.
From a machine learning engineer’s perspective, the key challenge is not model training, but reliably converting raw video streams into structured outputs that can support business decisions.

This project simulates that pipeline using a self-recorded video purely as a technical proof of concept.
The Python script used to process the video and perform object detection can be found here: [`detect_video.py`](detect_video.py).

# Business Use Cases
Although a personal video is used for demonstration, the same pipeline can be applied to real retail environments for:

- Customer presence detection
- Basic object and product visibility
- Operational monitoring
- Scalable AI deployment in headless environments

# Data & Model Overview

- Input: Short MP4 video clips (simulating in-store camera feeds OR self recorded MP4 video)
- Model: YOLOv8 Nano (pretrained on COCO dataset)
- Output:
    - Bounding boxes
    - Object labels
    - Confidence scores
    - Annotated video and GIF output
 
# Executive Summary
This project shows that pretrained object detection models can be integrated into a clean, reproducible pipeline that processes video data and generates explainable outputs.
Even with a simple demo video, the system demonstrates how unstructured visual data can be transformed into machine-readable signals suitable for business analytics.

# Demo Output:

# Key Observations

- YOLOv8 performs well on general object detection without task-specific training.
- Lightweight models are suitable for rapid prototyping and deployment.
- Video-to-GIF outputs make results easy to review and share with stakeholders.

# Recommendations

- Replace demo footage with in-store camera feeds for production use.
- Aggregate detections across time for operational insights.
- Extend the pipeline with behavior or action recognition modules.

# Assumptions & Limitations

- The demo video is self-recorded and non-retail, used only for validation.
- The model is not fine-tuned for specific store environments.
- Results are illustrative rather than production-calibrated.

# Tech Stack
- Python
- YOLOv8 (Ultralytics)
- OpenCV
- ImageIO
- Google Colab (headless execution)

# How to Run
pip install ultralytics opencv-python imageio
python detect_video.py

# Outputs:

- output.mp4 – annotated detection video
- demo.gif – GitHub-ready demo

# Final Note
This project focuses on practical ML engineering, demonstrating how computer vision models can be integrated into real-world business workflows with clean, reproducible code.
