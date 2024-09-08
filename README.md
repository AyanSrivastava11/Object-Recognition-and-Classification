# Objects Recognition and Classification
**Independent Project (ME499), Northwestern University, Winter 2021**

This project involves building neural networks to detect and classify objects in two primary categories: traffic signs and recyclable materials. It integrates computer vision techniques, using PyTorch, OpenCV, and YOLO, and also implements robotic solutions for recycling using the Baxter robot.


## Table of Contents
- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)

## Project Overview
This project is divided into two modules:

### 1. Traffic Sign Detection and Classification
In this module, I built and trained a neural network to detect and classify different traffic signs using **PyTorch**, **OpenCV**, and **YOLOv3**.

#### Traffic Sign Classification
- Built and trained a neural network to classify various traffic sign images.
- The model achieved high accuracy in distinguishing between different traffic signs based on image inputs.

#### Traffic Sign Detection
- Trained a neural network to detect different traffic signs within images and videos.
- Used YOLOv3 to identify and localize traffic signs with high precision.

**Example Output:**
![Traffic Detection Output](path/to/traffic_detection_image.png)

---

### 2. Trash Detection, Classification, and Segmentation
In this module, I built and trained a neural network to detect and classify various recyclable objects using **PyTorch**, **OpenCV**, and **YOLOv5**.

#### Trash Classification
- Developed a neural network to classify images of recyclable objects into categories like paper, plastic, and metal.
- Used PyTorch and YOLOv5 for training and prediction.

#### Trash Detection
- Trained a neural network to detect and classify recyclable objects in real-time from images and video inputs.

#### Segmentation
- Implemented segmentation techniques to outline detected recyclable objects, enabling further processing for robotic sorting.

**Example Output:**
![Trash Detection Output](path/to/trash_detection_image.png)

---

### 3. Recycling Baxter Implementation
This module extends the project by integrating the machine learning model with the Baxter robot. The robot detects, sorts, and locates recyclable objects using the neural network models trained in the previous modules.

- Implemented object detection algorithms to guide Baxter in picking up and sorting recyclable materials based on object type.

**Example of Recycling Baxter in Action:**
![Baxter Robot Sorting](path/to/baxter_robot_image.png)

---

## Technologies Used
- **Programming Languages**: Python
- **Libraries**: PyTorch, OpenCV, YOLOv3, YOLOv5, Numpy, Matplotlib
- **Tools**: Jupyter Notebooks, Google Colab
- **Robotics**: Baxter Robot

## Installation

### Prerequisites
- Python 3.x
- Pip
- PyTorch
- OpenCV

### Steps

1. Clone the repository:
    ```bash
    git clone <repository-link>
    ```

2. Navigate to the project directory:
    ```bash
    cd object-recognition-classification
    ```

3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Run the application:
    ```bash
    python app.py
    ```

## Usage

1. Use the `traffic_sign_detection.py` file for traffic sign detection and classification.
2. Use the `trash_detection.py` file for trash detection and segmentation.
3. The Baxter implementation can be run using the `baxter_implementation.py` file.

For further instructions on dataset usage, model training, and testing, refer to the individual module documentation in the repository.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
