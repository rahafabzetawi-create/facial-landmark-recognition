# Facial Landmark Detection and Person Class Creation

## 📌 Project Description

This project is designed to detect faces in images and extract the **68 facial landmarks** using the **Dlib** library.

The extracted facial landmark coordinates are used to represent each person's face and create a dataset that can be used for **facial recognition and classification**.

## 🎯 Project Objectives

The main objectives of this project are:

* Read multiple facial images for each person.
* Detect faces in the images.
* Detect **68 facial landmarks** using Dlib.
* Display the detected landmarks on the face.
* Extract the `(x, y)` coordinates of all 68 landmarks.
* Represent each face using its landmark coordinates.
* Organize the extracted data according to each person.
* Create a facial landmark dataset for recognition purposes.

## 🛠️ Technologies Used

* Python 3.11.9
* OpenCV
* Dlib
* NumPy
* Matplotlib
* Google Colab

## 📂 Project Structure

```text
Facial-Landmark-Detection/
│
├── images/
│   ├── person1/
│   ├── person2/
│   └── ...
│
├── shape_predictor_68_face_landmarks.dat
├── main.py
├── dataset.csv
└── README.md
```

## 🔍 How It Works

The project follows these main steps:

### 1. Read Images

Multiple images are loaded for each person from the dataset folders.

### 2. Face Detection

Dlib's face detector is used to locate faces in each image.

### 3. Facial Landmark Detection

The Dlib **68-point facial landmark predictor** detects important points on the face, including the eyes, eyebrows, nose, mouth, and jawline.

### 4. Landmark Extraction

For every detected face, the `(x, y)` coordinates of the 68 landmarks are extracted.

Each face is represented by:

```text
(x1, y1), (x2, y2), ..., (x68, y68)
```

### 5. Visualization

The detected landmarks are displayed on the original face image to verify that the detection works correctly.

### 6. Dataset Creation

The extracted coordinates are stored together with the person's identity to create a dataset suitable for further facial recognition tasks.

## 📊 Facial Landmarks

Dlib detects **68 facial landmark points**.

These points describe different facial regions such as:

* Jaw
* Eyebrows
* Eyes
* Nose
* Mouth

The landmark coordinates provide a numerical representation of the facial structure.

## ⚠️ Important Note

**Some code sections in this project are designed to run specifically in Google Colab and may not work correctly in a local Python environment without modifications.**

For the best compatibility, it is recommended to run the relevant code sections using **Google Colab**, especially the sections that depend on Colab-specific commands, paths, or environment configurations.

## ▶️ How to Run

### Using Google Colab

1. Open the project in Google Colab.
2. Upload the required images and files.
3. Make sure the file `shape_predictor_68_face_landmarks.dat` is available.
4. Run the code cells in order.

### Using a Local Python Environment

Install the required libraries:

```bash
pip install opencv-python numpy matplotlib dlib
```

Then run:

```bash
python main.py
```

> Note: Some parts of the project may require modifications when running locally instead of Google Colab.

## 📈 Output

The program produces:

* Detected faces.
* Images with the 68 facial landmarks displayed.
* `(x, y)` coordinates for each landmark.
* A dataset containing facial landmark features and person labels.

## 💡 Applications

Facial landmarks can be used in applications such as:

* Face recognition
* Face classification
* Facial expression analysis
* Face alignment
* Computer vision systems

## 👩‍💻 Author

**Rahaf Zetawi**

Data Science Student
