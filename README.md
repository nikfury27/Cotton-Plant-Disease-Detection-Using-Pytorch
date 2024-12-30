# Cotton Leaf Disease Detection using PyTorch

This project aims to detect diseases in cotton leaves using a convolutional neural network (CNN) built with PyTorch. The application provides a user-friendly interface for uploading images of cotton leaves or plants and identifying whether they are healthy or diseased.

---

## Table of Contents
- [Features](#features)
- [File Structure](#file-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Model Details](#model-details)

---

## Features
- **Disease Classification**: Detects diseases in cotton leaves and plants.
- **Web Interface**: Upload images via a web app built with Flask.
- **Model Training and Evaluation**: Train the model on your own dataset and evaluate its performance.

---

## File Structure
```
Cotton Disease Detection
├───.ipynb_checkpoints
├───data
│   ├───test
│   │   ├───diseased cotton leaf
│   │   ├───diseased cotton plant
│   │   ├───fresh cotton leaf
│   │   └───fresh cotton plant
│   ├───train
│   │   ├───diseased cotton leaf
│   │   ├───diseased cotton plant
│   │   ├───fresh cotton leaf
│   │   └───fresh cotton plant
│   └───val
│       ├───diseased cotton leaf
│       ├───diseased cotton plant
│       ├───fresh cotton leaf
│       └───fresh cotton plant
├───static
│   ├───css
│   └───js
├───templates
└───uploads
```

---

## Installation

Follow these steps to clone and set up the project locally:

### Prerequisites
- Python 3.10 or later
- pip package manager
- Virtual environment (optional but recommended)

### Clone the Repository
```bash
$ git clone https://github.com/your-username/cotton-leaf-disease-detection.git
$ cd cotton-leaf-disease-detection
```

### Set Up a Virtual Environment (Optional)
```bash
$ python -m venv venv
$ source venv/bin/activate   # On Windows: venv\Scripts\activate
```


---

## Usage

### 1. Prepare the Dataset
Ensure the dataset is in the `data/` directory, organized into `train`, `val`, and `test` subdirectories, as described in the file structure above.

### 2. Use the Pre-Trained Model

```bash
modelCottonDemo.pth
```

### 3. Run the Application
Start the Flask application:
```bash
$ python app.py
```
Open your browser and navigate to `http://127.0.0.1:5000` to access the web interface.

### 4. Test the Model
Upload images through the web interface to classify them as healthy or diseased.

---

## Dataset
You can download the dataset <a href="https://www.kaggle.com/datasets/janmejaybhoi/cotton-disease-dataset">here</a>.
It's a tiny dataset with 4 classes.

The dataset should be structured as follows:
- `train/`: Contains training data.
- `val/`: Contains validation data.
- `test/`: Contains testing data.

Each folder should have subfolders for the four categories:
- Diseased Cotton Leaf
- Diseased Cotton Plant
- Fresh Cotton Leaf
- Fresh Cotton Plant

---

## Model Details
- **Architecture**: Convolutional Neural Network (CNN)
- **Framework**: PyTorch
- **Preprocessing**: Images are resized and normalized before being fed into the model.

---


Feel free to raise issues or contribute to this project by submitting pull requests. Happy coding!

