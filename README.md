# Traffic-Sign-Detection-Under-Different-Weather-Conditions-using-YOLOv11

This project focuses on detecting traffic signs in diverse weather conditions using the YOLOv11 object detection architecture. The primary goal is to evaluate the robustness and accuracy of YOLOv11 when trained and tested on datasets containing weather variations like rain, fog, and snow.

🧠 Overview

Model: YOLOv11

Task: Object Detection (Traffic Sign Detection)

Dataset: Augmented traffic sign dataset with multiple weather conditions

Framework: PyTorch + OpenCV + Ultralytics YOLO

Goal: Improve and evaluate detection accuracy under challenging visual environments

📁 Project Structure
```
Traffic Sign Detection/
|-- Night/
|-- Normal/
|-- Rain/
|-- Snow/
```
⚙️ Installation

# Clone the repository
```
git clone https://github.com/Hemanth-Katikala-Muniraj/Traffic-Sign-Detection-Under-Different-Weather-Conditions-using-YOLOv11-.git

cd Traffic-Sign-Detection-Under-Different-Weather-Conditions-using-YOLOv11-
```
# Create a virtual environment 
```
python -m venv venv

source venv/bin/activate  

# On Windows: venv\Scripts\activate
```
# Install dependencies

```
pip install -r requirements.txt
```

🏃‍♂️ Usage

1. Train the model

```
python scripts/train.py --data data/dataset.yaml --cfg yolov11.yaml --weights '' --epochs 50
```
2. Run inference

```
python scripts/detect.py --weights runs/weights/best.pt --source data/test/images
```
📊 Evaluation

Evaluation metrics include:

- mAP@0.5
- Precision, Recall
- Per-class AP under different weather conditions
- Results are saved in the results/ directory.

🧪 Dataset

The dataset used includes traffic sign images augmented with synthetic weather effects (rain, fog, snow) to simulate real-world driving scenarios. Dataset annotations follow YOLO format.

🛠️ Dependencies

- Python 3.8+
- PyTorch
- OpenCV
- Ultralytics YOLOv11
- Albumentations

Install all dependencies using:
pip install -r requirements.txt

📌 Acknowledgements

- Ultralytics YOLO
- OpenCV
- Albumentations

📃 License

This project is licensed under the MIT License.
