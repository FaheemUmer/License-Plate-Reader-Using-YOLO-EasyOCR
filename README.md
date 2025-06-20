# License Plate Detector and Reader using YOLOv5 + EasyOCR

This project detects and reads vehicle license plates from images and videos using a combination of **YOLOv5** (for object detection) and **EasyOCR** (for Optical Character Recognition). It can be used for surveillance, traffic monitoring, smart parking, or toll systems.

---

## 🚀 Features

- Fast and accurate license plate detection using YOLOv5  
- Text extraction from plates using EasyOCR  
- Works on both images and videos  
- Trained on a real-world annotated dataset from Roboflow Universe  
- Saves processed outputs with bounding boxes and recognized text  

---

## ⚙️ How It Works

### 1. License Plate Detection (YOLOv5)

The project uses **YOLOv5**, a real-time object detection model, trained specifically to detect license plates in images and video frames.

- **Dataset**: [License Plate Recognition – Roboflow Universe](https://universe.roboflow.com/yolov5-sg5le/license_plate_recognition-qslmk/dataset/6)  
- **Model**: YOLOv5 custom-trained model (`best.pt`)  
- **Output**: Bounding boxes with confidence scores for detected plates  

### 2. Text Recognition (EasyOCR)

After detecting and cropping the license plate regions, the system uses **EasyOCR** to read the characters on the plate.

- Works well with alphanumeric characters  
- Handles various plate fonts and lighting conditions  
- Outputs the extracted text overlaid on the image or video frame  

---

## 🖼️ Sample Outputs

![output1](https://github.com/user-attachments/assets/034468d8-5cfb-40ea-9407-fc50481c1b28)  
![output2](https://github.com/user-attachments/assets/4b1e5440-ecb0-4237-84d5-c0fd2c3de8bd)  
![output3](https://github.com/user-attachments/assets/d0847023-9b5f-4a0d-b644-879465bbb6c9)

---

## 📁 Project Structure

```bash
.
├── License_Plate_Detector_and_Reader.ipynb   # Main Jupyter Notebook
├── best.pt                                   # YOLOv5 trained weights 
├── requirements.txt                          # Python dependencies
└── README.md                                 # Project documentation

## 🔮 Future Enhancements

- Integrate webcam support for real-time plate detection  
- Improve accuracy on low-light or motion-blur images  
- Add support for multilingual and regional plates  
- Store recognized plates in a searchable database  
- Create a dashboard to view and manage detected vehicles  
- Add vehicle type detection (car, bike, truck)  
- Deploy using Flask or FastAPI for web-based interaction  
- Batch process folders of images and videos  


