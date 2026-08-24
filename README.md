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
Trained and evaluated on the curated 2,000+ smartphone screen defects dataset[cite: 1]:

 Class     Images  Instances    Box(P)       R          mAP50     mAP50-95
  all        302        424      0.906      0.905      0.928      0.762
  dot         59        162      0.801      0.833      0.863      0.497
scratch       55        216       0.96       0.88       0.93      0.832
 crack        46         46      0.958          1       0.99      0.956

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
