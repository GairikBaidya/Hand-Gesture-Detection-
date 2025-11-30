# 🖐️ Hand Gesture Recognition System

> **A Deep Learning project to recognize and classify hand gestures in real-time.**

---

## 📖 About The Project

This project implements a **Convolutional Neural Network (CNN)** capable of identifying 10 different hand gestures from images. It's designed to be the core engine for applications like:
*   **Touchless Interfaces**: Controlling computers or kiosks with hand waves.
*   **Sign Language Recognition**: Translating basic hand signs into text.
*   **Gaming Controls**: Using hand movements as input.

The model is built using **Python** and **TensorFlow/Keras**, making it robust and easy to extend.

---

## 🚀 Key Features

*   **10-Class Recognition**: Can distinguish between gestures like *Palm*, *Fist*, *Thumb*, *Index*, *OK*, and more.
*   **High Accuracy**: Uses a custom CNN architecture optimized for image classification.
*   **Data Preprocessing**: Automatically handles image resizing (100x100), grayscale conversion, and normalization.
*   **Visualizations**: Includes built-in tools to visualize training progress (accuracy/loss graphs) and sample predictions.

---

## 🛠️ Technologies Used

*   ![Python](https://img.shields.io/badge/Python-3.8%2B-blue) **Python**: The core programming language.
*   ![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-orange) **TensorFlow & Keras**: For building and training the deep learning model.
*   ![NumPy](https://img.shields.io/badge/NumPy-Data-lightblue) **NumPy**: For efficient numerical operations.
*   ![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-green) **Matplotlib**: For plotting graphs and displaying images.

---

## 🧠 How It Works

1.  **Input**: The system takes a grayscale image of a hand.
2.  **Processing**: The image is resized to 100x100 pixels and converted to a format the AI can understand.
3.  **Analysis**: The **CNN** (Convolutional Neural Network) scans the image for patterns like edges, curves, and shapes.
4.  **Prediction**: The model calculates the probability for each of the 10 gestures and outputs the most likely one.

### The 10 Gestures
| ID | Gesture Name | Description |
| :--- | :--- | :--- |
| `0` | **Palm** | Open hand facing forward |
| `1` | **I** | The letter 'I' or pinky extended |
| `2` | **Fist** | Closed hand |
| `3` | **Fist (moved)** | Fist in motion |
| `4` | **Thumb** | Thumbs up |
| `5` | **Index** | Index finger pointing |
| `6` | **OK** | OK sign |
| `7` | **Palm (moved)** | Open hand in motion |
| `8` | **C** | The letter 'C' shape |
| `9` | **Down** | Hand pointing down |

---

## 📂 Project Structure

```text
project_sem6/
├── README.md           # This documentation file
├── project_sem6.py     # The main Python script (Training & Evaluation)
└── leapGestRecog/      # (Required) Folder containing the dataset
    ├── 00/             # Images for subject 1
    ├── 01/             # Images for subject 2
    └── ...
```

---

## ⚡ Getting Started

### Prerequisites
You need Python installed along with the following libraries:
```bash
pip install tensorflow numpy matplotlib scikit-learn pillow
```

### Running the Project
1.  **Download the Dataset**: This project requires the **LeapGestRecog** dataset (typically available on Kaggle).
2.  **Place the Data**: Extract the dataset so that a `leapGestRecog` folder exists in the same directory as the script.
3.  **Run the Script**:
    ```bash
    Hand-Gesture-Detection.py
    ```

> **Note**: The current script contains some code specific to Google Colab (like `google.colab` imports). These sections need to be commented out or removed to run locally on your machine.
