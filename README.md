---

# P&ID Component Detection

This repository contains a Jupyter Notebook (`Yolo.ipynb`) demonstrating the implementation of the **YOLO (You Only Look Once)** object detection algorithm. YOLO is a popular and efficient deep learning model for real-time object detection in images and videos.

---

## Dataset
Dataset is obtained from Roboflow universe consisting of all the related p&id components images with their interconnections

- Consisting of both individual components and interconnected components
- Custom Data Augumentation is done for improvising the model performance.
- **Data Augumentation** includes:
  
  1. Resize
  2. Rotations
  3. Guassian Noise
  4. Salt and Pepper Noise
  5. Varrying brightness 
  6. Colored Images
---

## Features

- **Object Detection**: Detects multiple objects in images or video frames with bounding boxes and class labels.
- **YOLO Framework**: Utilizes YOLO for fast and accurate detection.
- **Customizable**: Easily adaptable to new datasets and configurations.
- **Visualization**: Outputs images with detected objects highlighted by bounding boxes.

---

## Prerequisites

### Libraries Required
Ensure you have the following Python libraries installed before running the notebook:

- `numpy`
- `opencv-python`
- `torch`
- `torchvision`
- `matplotlib`
- `Pillow` (for image handling)
- `yolov5` (if leveraging pre-trained YOLO models from Ultralytics)

You can install the required libraries using pip:
```bash
pip install numpy opencv-python torch torchvision matplotlib Pillow yolov5
```

---

## Usage

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/yolo-implementation.git
   cd yolo-implementation
   ```

2. **Open the Notebook**:
   Launch Jupyter Notebook or JupyterLab in your terminal:
   ```bash
   jupyter notebook Yolo.ipynb
   ```

3. **Prepare Input Data**:
   - Add images or videos for object detection in a designated `data/` directory.
   - Ensure paths in the notebook point to your data files.

4. **Run the Notebook**:
   - Step through the cells sequentially to:
     - Load YOLO models (pre-trained or custom-trained).
     - Perform object detection on the input data.
     - Visualize and save the results.

5. **Modify for Custom Use Cases**:
   - Replace the dataset or adjust YOLO configuration (e.g., anchors, confidence thresholds).
   - Train the YOLO model on the auguemented dataset available after performing data augumentation from Roboflow. 

---

## Example Output

The notebook will output images or video frames with detected objects marked by bounding boxes and labeled with class names. 

Example Output:


![YOLO Output Example](/runs/detect/predict/154_png_jpg.rf.f42d1535616534054de725a9bb75c54f.jpg)

---

## Notes

- Ensure GPU support is enabled for faster processing, especially for large datasets.
- For custom training, follow the dataset preparation guidelines for YOLO (e.g., COCO format).

---
