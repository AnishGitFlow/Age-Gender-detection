
### Age and Gender Detection

This project uses OpenCV and deep learning models to detect faces in real-time using a webcam or from image files, and predict the age and gender of the detected faces.

### Table of Contents
- [Features](#features)
- [Requirements](#requirements)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Models and Files](#models-and-files)
- [License](#license)

### Features
- Real-time age and gender detection using webcam.
- Ability to analyze static images.
- Utilizes deep learning models for face detection and age/gender prediction.

### Requirements
- **Python 3.x**
- **OpenCV**
- **NumPy**

You can install the required packages using `pip`:

```bash
pip install opencv-python opencv-python-headless numpy
```

### Setup Instructions

#### Step 1: Clone the Repository

```bash
git clone https://github.com/AnishGitFlow/age-gender-detection.git
cd age-gender-detection
```

#### Step 2: Download the Model Files
I have not added the following two model files to the repository. You will need to download them manually from the internet:

1. **Age Detection Model**
   - **Age Prototxt file (age_deploy.prototxt):**
   - **Age Model (age_net.caffemodel):**

2. **Gender Detection Model**
   - **Gender Prototxt file (gender_deploy.prototxt):**
   - **Gender Model (gender_net.caffemodel):**

Make sure to place these files in the same directory as your Python script.

#### Step 3: Place Your Image Files
If you want to test with images, ensure they are in the same folder or provide the path to them.

### Usage

#### To Run the Script Using Webcam
Execute the following command in your terminal:

```bash
python Age.py --image 0
```

#### To Run the Script Using an Image File
Specify the image path:

```bash
python Age.py --image path_to_image.jpg
```

Replace `path_to_image.jpg` with the actual name of your image file.

### Exit the Application
Press `q` while the window is active to exit the application.

### Models and Files

The following files are used for face detection, age prediction, and gender prediction:

- **Face Detection**:
  - `opencv_face_detector.pbtxt`
  - `opencv_face_detector_uint8.pb`

- **Age Detection**:
  - `age_deploy.prototxt`
  - `age_net.caffemodel` (Download from the link provided)

- **Gender Detection**:
  - `gender_deploy.prototxt`
  - `gender_net.caffemodel` (Download from the link provided)

Ensure all these files are available in the same directory as the script for it to run correctly.
