# AI-Powered-Video-Object-Detection-for-Retail-Intelligence
This repository demonstrates an end-to-end computer vision system that applies real-time object detection to retail video footage, with a focus on business insights, operational intelligence, and production readiness.

The goal is to show how machine learning can move beyond experimentation into decision-support systems used by retail operations, loss prevention, and store analytics teams.

# Project Background
Business Context

The project is framed around a retail technology company operating in the physical retail analytics and AI services industry. The company provides AI-driven video intelligence solutions to brick-and-mortar retailers to improve store operations, customer experience, and asset utilization.

From a Machine Learning Engineer’s perspective, the system is designed to:

- Process in-store video feeds
- Detect and classify physical objects in real time
- Generate structured data from unstructured video streams
- Enable downstream analytics and business decision-making

# Business Use Cases

This solution can support several practical retail scenarios:

- Customer presence monitoring (footfall estimation)
- Basic inventory visibility (product presence on shelves)
- Store safety and operations monitoring
- Scalable AI deployment using lightweight models

# Data & Model Overview

- Input: Short MP4 video clips (simulating in-store camera feeds)
- Model: YOLOv8 Nano (pretrained on COCO dataset)
- Output:
    - Bounding boxes
    - Object labels
    - Confidence scores
    - Annotated video and GIF output
 
# Executive Summary
The project shows that pretrained computer vision models can reliably extract useful signals from retail video streams with minimal setup.
By converting unstructured video into structured detections, retailers can enable data-driven decisions without changing existing camera infrastructure.

# Demo Output:

# Key Observations

- Object detection works effectively on short retail-like video clips.
- Lightweight models (YOLOv8n) are suitable for real-time or near-real-time use.
- Video outputs and GIFs provide clear, explainable results for non-technical stakeholders.

# Recommendations

- Use lightweight object detection models for cost-efficient deployment.
- Aggregate detections over time to derive higher-level KPIs (e.g., traffic trends).
- Extend the pipeline with behavior or action recognition for deeper insights.

# Assumptions & Limitations

- The model is pretrained and not fine-tuned on store-specific data.
- Detections are used as indicators, not exact measurements.
- Demo videos are representative but not exhaustive of real retail environments.

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
