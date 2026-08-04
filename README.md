# Real-Time Sign Language Detection using TensorFlow Object Detection

## Overview

This project is a real-time Sign Language Detection system developed using the TensorFlow Object Detection API, SSD MobileNet, and OpenCV. It recognizes predefined sign language gestures from a live webcam feed and displays the predicted sign in real time.

The project demonstrates the complete deep learning pipeline, including data collection, image annotation, TFRecord generation, model training, and real-time inference.

## Features

* Real-time sign language detection using a webcam
* Custom dataset collection
* Image annotation using LabelImg
* TensorFlow Object Detection API
* SSD MobileNet object detection model
* Live bounding box visualization
* Confidence score display
* Easily extendable to additional sign classes

## Sign Classes

The model is trained to recognize the following signs:

* Hello
* Yes
* No
* Thank You
* I Love You

## Tech Stack

* Python
* TensorFlow 2
* TensorFlow Object Detection API
* OpenCV
* NumPy
* Protobuf
* LabelImg

## Project Structure

```text
Tensorflow/
│
├── workspace/
│   ├── annotations/
│   ├── images/
│   │   ├── train/
│   │   └── test/
│   ├── models/
│   └── pre-trained-models/
│
├── models/
│   └── research/
│
└── scripts/
```

## Workflow

1. Collect images for each sign.
2. Annotate images using LabelImg.
3. Generate TFRecord files.
4. Configure the SSD MobileNet pipeline.
5. Train the object detection model.
6. Export the trained model.
7. Perform real-time sign detection using a webcam.

## Results

The trained model successfully detects supported sign language gestures in real time with bounding boxes and confidence scores.

## Future Improvements

* Support continuous sign language sentence recognition.
* Replace SSD MobileNet with MediaPipe Hands for improved speed and efficiency.
* Train an LSTM or Transformer model for sequence-based recognition.
* Add speech synthesis (Text-to-Speech).
* Translate recognized signs into complete English or Urdu sentences.
* Deploy the application as a web or mobile application.

## Acknowledgements

This project was implemented by following the concepts presented in the tutorial:

**Real Time Sign Language Detection with TensorFlow Object Detection and Python | Deep Learning SSD**

The implementation was customized for a personal sign language recognition dataset and end-to-end training pipeline.

## License

This project is intended for educational and research purposes.
