# Emotion Detection using OpenCV and TensorFlow

This project demonstrates a real-time facial emotion recognition system built with TensorFlow, using transfer learning with MobileNetV2 and OpenCV for webcam integration.

## Features

- Real-time emotion detection via webcam
- Transfer learning with MobileNetV2
- Automatic face detection using OpenCV's Haar cascades
- Data augmentation using Keras' `ImageDataGenerator`
- Multi-class emotion classification (e.g., Happy, Sad, Angry, etc.)

## Technologies Used

- **TensorFlow** / **Keras**: For model building and training
- **OpenCV**: For video capture and face detection
- **MobileNetV2**: Pre-trained model for transfer learning
- **NumPy** / **Matplotlib**: For array operations and visualization

## Directory Structure

```
project/
├── data/
│   ├── train/
│   │   ├── angry/
│   │   ├── happy/
│   │   └── ... (emotion class folders)
│   └── validation/
│       ├── angry/
│       ├── happy/
│       └── ...
├── Emotion_Detection_TensorFlow_OpenCV.ipynb
└── README.md
```

## Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/rebantamandal/emotion-detection-tf-opencv.git
cd emotion-detection-tf-opencv
```

### 2. Install Dependencies
```bash
pip install tensorflow opencv-python matplotlib
```

### 3. Organize Dataset
Create the following folder structure and add your emotion-labeled images:
```
data/
├── train/
│   ├── angry/
│   ├── happy/
│   └── ...
├── validation/
│   ├── angry/
│   ├── happy/
│   └── ...
```

### 4. Run the Notebook
Open and run the notebook:
```
Emotion_Detection_TensorFlow_OpenCV.ipynb
```

### 5. Start Real-Time Detection
After training and saving the model:
- The final cell in the notebook uses OpenCV to launch your webcam.
- Detected faces will display the predicted emotion label in real time.
- Press `q` to quit the webcam window.

## Notes

- Make sure your webcam is enabled.
- Use a dataset with at least a few hundred images per emotion class for better accuracy.
- Fine-tune the model or unfreeze some MobileNetV2 layers for improved performance.

## License

This project is released under the MIT License.
