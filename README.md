# 🚗 Autonomous Driving - Car Detection

This repository implements a car detection system using the YOLO (You Only Look Once) algorithm. YOLO is a state-of-the-art object detection model known for its speed and accuracy. The code demonstrates the use of TensorFlow and Keras to filter and visualize bounding boxes for detecting cars in an image.

---

## 🛠️ Features
- Implementation of the YOLO algorithm for car detection.
- Functions for filtering bounding boxes based on confidence scores.
- Non-Maximum Suppression (NMS) to eliminate redundant boxes.
- Utilities for preprocessing, scaling, and drawing boxes on images.
- Interactive testing with TensorFlow and Python.

---

## 📁 Directory Structure
- **`yolo_utils.py`**: Utility functions for reading classes, anchors, preprocessing images, and drawing bounding boxes.
- **`yad2k.models.keras_yolo.py`**: Prebuilt YOLO model architecture for Keras.

---

## 📝 Problem Statement
Detect and localize cars in an input image by:
1. Identifying bounding boxes using YOLO.
2. Filtering and refining predictions through confidence thresholds and NMS.
3. Visualizing the results on the image.

---

## 📚 Code Overview

### 1️⃣ YOLO Algorithm
YOLO divides the input image into a grid and predicts bounding boxes for detected objects. Each bounding box is associated with:
- **Class scores**: Probability of belonging to a specific class.
- **Bounding box coordinates**: Location and size of the box.

---

### 2️⃣ Key Functions

#### 🔎 `yolo_filter_boxes()`
Filters boxes by applying a confidence threshold to discard low-probability detections.

#### ✂️ `iou()`
Computes the Intersection over Union (IoU) for two bounding boxes, a metric to evaluate overlap.

#### 🚫 `yolo_non_max_suppression()`
Applies NMS to remove overlapping bounding boxes and retain the most relevant ones.

#### 🖼️ `yolo_eval()`
Wraps up filtering and NMS to produce final predictions (scores, boxes, and classes).

---

## 📊 Example Output
Tested on random input tensors, the following results demonstrate the workflow:
- Filtered bounding boxes.
- Non-overlapping boxes after NMS.
- Final confidence scores.

---

## 💻 Requirements
- Python 3.7+
- TensorFlow 2.x
- Keras
- NumPy
- Matplotlib
- PIL (Pillow)

Install the dependencies using:
```bash
pip install -r requirements.txt
```

---

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/autonomous-driving-car-detection.git
   cd autonomous-driving-car-detection
   ```
2. Run the example scripts provided to test various functionalities.

---

## 🎓 Credits
This repository is inspired by the Deep Learning Specialization by [DeepLearning.AI](https://www.deeplearning.ai/courses/deep-learning-specialization/). The YOLO implementation and techniques used here are aligned with their teachings. A special thanks to the creators for their exceptional resources. 🌟

---

## 🛡️ License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 🌟 Contributions
Contributions are welcome! Feel free to fork this repository, open issues, or submit pull requests.

---

### 📬 Contact
For queries or collaboration, feel free to reach out via https://www.upwork.com/freelancers/~01c49d81acd187f26f
