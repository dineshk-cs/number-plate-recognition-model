🚗 Number Plate Recognition System
📌 Project Description

This project is a basic Number Plate Recognition (NPR) system developed using Python.
It detects vehicles, identifies number plates, and extracts the plate number using deep learning and OCR techniques.

🛠️ Technologies Used

> Python
> YOLOv8 (from Ultralytics)
> OpenCV (from OpenCV)
> EasyOCR
> Google Colab
 
🎯 Features

> Detects vehicles (Car / Motorcycle)
> Detects number plates
> Extracts text from number plates

📂 Project Structure

project-folder/
│
├── dataset/
├── runs/
├── number_plate_recognition.ipynb
├── best.pt
└── README.md

🚀 How to Run
1️⃣ Install Required Libraries
pip install ultralytics
pip install opencv-python
pip install easyocr

2️⃣ Train the Mode
from ultralytics import YOLO

model = YOLO("yolov8s.pt")
model.train(data="dataset/data.yaml", epochs=50)

3️⃣ Run Detection
model = YOLO("best.pt")
results = model("test_image.jpg")

📖 How It Works

> Input image is given to the model
> YOLO detects vehicle and number plate
> Plate region is cropped
> EasyOCR extracts text

📌 Applications

> Smart Parking System
> College / Office Entry System
> Toll Gate Automation



