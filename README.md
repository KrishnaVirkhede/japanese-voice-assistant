# 🎥 Real-Time Object Detection with YOLOv8

A real-time object detection system using YOLOv8 and OpenCV for live webcam feed analysis.

## ✨ Features

- 🎯 **Real-time Object Detection** using YOLOv8n model
- 📹 **Live Webcam Integration** for continuous monitoring
- 🎨 **Visual Annotations** with bounding boxes and labels
- 📊 **Confidence Scores** displayed for each detection
- ⚡ **Optimized Performance** for real-time processing
- 🔄 **80+ Object Classes** detection capability (COCO dataset)

## 🛠️ Technologies Used

- **Python 3.x**
- **OpenCV (cv2)** - Computer vision and video processing
- **Ultralytics YOLOv8** - State-of-the-art object detection
- **YOLOv8n** - Nano model for fast inference

## 📋 Prerequisites

```bash
pip install opencv-python
pip install ultralytics
```

## 🚀 How to Run

1. Clone this repository:
```bash
git clone https://github.com/KrishnaVirkhede/yolov8-object-detection.git
cd yolov8-object-detection
```

2. Run the detector:
```bash
python MoreAdvanceTCDS.py
```

3. Press **'q'** to quit the application

## 🎯 Detectable Objects

The model can detect 80 different object classes including:
- 👤 People
- 🚗 Vehicles (car, truck, bus, motorcycle, bicycle)
- 🐕 Animals (dog, cat, bird, horse, etc.)
- 📱 Electronics (phone, laptop, keyboard, mouse)
- 🪑 Furniture (chair, table, couch, bed)
- And many more!

## 📂 Project Structure

```
yolov8-object-detection/
│
├── MoreAdvanceTCDS.py  # Main detection script
├── yolov8n.pt          # YOLOv8 nano model (auto-downloaded)
└── README.md           # Project documentation
```

## 🔧 How It Works

1. **Model Loading**: Loads pre-trained YOLOv8n model
2. **Video Capture**: Connects to default webcam (index 0)
3. **Frame Processing**: Each frame is fed to YOLO for inference
4. **Visualization**: Results are annotated with bounding boxes and labels
5. **Display**: Processed frames shown in real-time window

## ⚙️ Customization

### Use Different Camera
```python
cap = cv2.VideoCapture(1)  # Change to 1, 2, etc. for other cameras
```

### Use Larger Model (Better Accuracy)
```python
model = YOLO("yolov8s.pt")  # Small model
model = YOLO("yolov8m.pt")  # Medium model
model = YOLO("yolov8l.pt")  # Large model
```

### Process Video File Instead of Webcam
```python
cap = cv2.VideoCapture("path/to/video.mp4")
```

## 📊 Performance

- **Model**: YOLOv8n (Nano)
- **Speed**: 30+ FPS on modern hardware
- **Accuracy**: mAP 37.3 on COCO dataset
- **Model Size**: ~6 MB

## 🎯 Future Improvements

- [ ] Add object tracking across frames
- [ ] Implement custom object detection training
- [ ] Save detection results to file
- [ ] Add GUI with detection controls
- [ ] Multi-camera support
- [ ] Detection alerts for specific objects

## 👤 Author

**Krishna Virkhede**
- GitHub: [@KrishnaVirkhede](https://github.com/KrishnaVirkhede)
- LinkedIn: [Krishna Virkhede](https://www.linkedin.com/in/krishna-virkhede-b600a6317)

## 📚 Resources

- [Ultralytics YOLOv8 Documentation](https://docs.ultralytics.com/)
- [OpenCV Documentation](https://docs.opencv.org/)

## 📄 License

This project is open source and available for educational purposes.

---

⭐ If you found this project helpful, please give it a star!
