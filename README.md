ScreenSense AI: Automated Smartphone Screen Defect Detection

Project Overview
ScreenSense AI is an end-to-end automated optical inspection (AOI) solution designed to democratize cosmetic quality assurance for the secondary smartphone and repair market. By replacing error-prone, subjective manual inspection with modern computer vision, the platform delivers high-accuracy defect localization and automated digital condition verification.

AI & Detection Architecture
- Model Architecture: YOLOv12l Object Detection Core
- Target Defect Classes:
  - Cracks: Structural glass fissures and impact fractures.
  - Scratches: Surface-level hairline abrasions and cosmetic wear.
  - Dots: Localized display spots, contamination, and pixel anomalies.
- AI Microservice: Python/Flask engine containerized with Docker and deployed for isolated GPU/CPU inferencing.

Benchmark & Evaluation Metrics

Trained and evaluated on the curated 2,000+ smartphone screen defects dataset:

OVERALL SUMMARY METRICS

Overall mAP50:    0.9276
Overall mAP50-95: 0.7618
Mean Precision:   0.9063
Mean Recall:      0.9046
Model Fitness:    0.7618

- Inference Speed: ~25.9 ms per image
- Preprocessing / Postprocessing: ~1.2 ms / ~0.5 ms

 System Architecture & Responsibilities

 AI Intelligence Layer
- Lead Developer: Malik Muqeet | Data Engineering & AI Architecture
- Dataset Pipeline: Dataset aggregation, multi-source pooling, labeling, and preprocessing.
- Model Training: YOLOv12-L fine-tuning, hyperparameter optimization, and class-imbalance mitigations.
- Microservice: Standalone Python/Flask engine containerized with Docker for GPU/CPU acceleration.
- Artifacts:
- [Kaggle Notebook] https://www.kaggle.com/code/malikmuqeet/mobile-screen-defect-detection-yolov12l
- [Kaggle Dataset]  https://www.kaggle.com/datasets/malikmuqeet/mobile-phone-screen-defects-dataset
- [Live Website]    https://www.screensenseai.me/
