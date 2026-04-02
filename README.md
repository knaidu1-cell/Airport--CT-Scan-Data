YOLO Threat Detection for CT Scan & Baggage Images

This project is a computer vision system for airport security that detects potential threats in baggage or CT scan images using YOLOv8. It is designed to help security personnel quickly and accurately identify dangerous items or suspicious patterns in real-time.

Key Objectives
Automate Threat Detection: Classify images into ThreatsRGB, HighLow, and Non-Threats, reducing the manual effort in baggage inspection.
Robust Model Training: Fine-tune a pretrained YOLOv8 model on a custom dataset of CT scans and baggage images.
Interactive Demo: Provide a simple interface where users can upload images and immediately see annotated predictions.
How It Works
Data Preparation
Original CT scan and baggage images are split into train, validation, and test sets.
Images are resized, normalized, and augmented to improve model robustness.
.tif images are converted to .jpg for compatibility with YOLOv8.
YOLOv8 Model Training
Uses YOLOv8n (small) pretrained model for classification.
Model is trained on the dataset with data augmentation for better generalization.
Fine-tuning improves accuracy for minority classes like Non-Threats or HighLow categories.
Model Evaluation
Predicts each test image and evaluates using:
Overall Accuracy
Classification Report (precision, recall, F1-score)
Confusion Matrix
Ensures the model reliably distinguishes threats from non-threats.
Interactive Prediction
Users can upload an image via Gradio interface.
The model returns the predicted class along with a visual annotated image, showing detected regions and threat classification.
Why It Matters
Helps security teams quickly flag suspicious items in baggage or CT scans.
Reduces human error in threat detection.
Can be deployed as a web-based demo for real-world evaluation by stakeholders.
Future Improvements
Integrate with airport X-ray machines for live scanning.
Optimize model for GPU deployment for faster inference.
Expand dataset for more diverse threat categories to improve robustness.
