## 🧠 Handwritten Digit Recognizer with CNN

This project implements a Convolutional Neural Network (CNN) in Python using TensorFlow/Keras to recognize handwritten digits from images. It uses a preprocessed dataset (similar to MNIST) and allows users to test the trained model with their own images.

---

### 📁 Project Structure

```
handwritten_digit_recognizer/
│
├── train_model.py                # Code to train the CNN model
├── digit_cnn_model.h5            # Saved trained CNN model
├── predict_digit.py              # Script to predict digit from user input image
├── handwritten_dataset.csv       # Custom preprocessed dataset
├── utils/                        # (Optional) helper functions
│
├── README.md                     # Project documentation
└── requirements.txt              # Python dependencies
```

---

### 📦 Requirements

Install required libraries via pip:

```bash
pip install -r requirements.txt
```

**requirements.txt**

```txt
tensorflow
pillow
numpy
matplotlib
```

---

### 🚀 How to Run

#### 🔧 Step 1: Train the Model (if not already trained)

```bash
python train_model.py
```

> This will train a CNN model and save it as `digit_cnn_model.h5`.

#### 📸 Step 2: Predict a Digit from an Image

Make sure your image is:

* In grayscale or RGB format
* Clearly shows a single digit (0–9)
* At least 28x28 pixels in size

```bash
python predict_digit.py
```

The script will:

1. Ask for the image path
2. Preprocess the image
3. Predict the digit
4. Show the result with a visual

---

### 🧪 Dataset

You can use your own dataset in CSV format (`handwritten_dataset.csv`) where each row contains:

* **Label** (first column): The true digit (0–9)
* **Pixels** (rest of the columns): 784 values representing a 28×28 image

---

### 🖼️ Sample Prediction Output

<img src="https://upload.wikimedia.org/wikipedia/commons/2/27/MnistExamples.png" width="300"/>

---

### ✅ Features

* Trained on high-quality digit images
* Accepts user input images
* Automatically preprocesses (resize, invert, normalize)
* Visual feedback of prediction
* Extendable to live webcam input or GUI

---

### 🧰 Future Improvements

* GUI using Tkinter or Streamlit
* Real-time prediction using webcam
* Train on more diverse handwriting samples
* Auto-centering and padding of digits

---

### 👨‍💻 Author

Raghavendra N
📫 *Built as part of Codec Technologies Internship Project*

