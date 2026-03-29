🚗 Driver Drowsiness Detection System

📌 Project Overview

This project aims to detect driver drowsiness using deep learning techniques.
It classifies driver eye and mouth states into four categories and further maps them into fatigue levels such as Alert, Mild Fatigue, and Severe Fatigue.

This system helps improve road safety by identifying early signs of driver fatigue.

---

🎯 Objectives

- Detect driver eye state (open / closed)
- Identify yawning behavior
- Classify images into 4 categories
- Convert predictions into fatigue levels
- Improve driver safety using AI

---

🛠️ Technologies Used

- Python
- TensorFlow / Keras
- MobileNetV2
- OpenCV
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

📂 Dataset Details

The dataset consists of images categorized into 4 classes:

- Open
- Closed
- Yawn
- No Yawn

Images are preprocessed and augmented using ImageDataGenerator.

---

⚙️ Model Architecture

- Base Model: MobileNetV2 (pretrained on ImageNet)
- Input Size: 224 x 224 x 3
- Layers Added:
  - GlobalAveragePooling2D
  - Dense (128, ReLU)
  - Dense (4, Softmax)

---

🧪 Training Details

- Loss Function: Categorical Crossentropy
- Optimizer: Adam
- Epochs: 5
- Training Accuracy: ~90%

---

📊 Model Evaluation

✔ Classification Report

- Precision, Recall, F1-score calculated for all classes

✔ Confusion Matrix

- Visualized using heatmap

✔ Accuracy Graph

- Training vs Validation accuracy plotted

---

🧠 Fatigue Detection Logic

Class| Fatigue Level
Open| Alert
No Yawn| Alert
Yawn| Mild Fatigue
Closed| Severe Fatigue

---

🔍 Sample Prediction

Example output:

Predicted Class: Open  
Fatigue Level: Alert

---

💾 Files Included

- "Driver_Drowsiness_Detection_project.ipynb"
- "drowsiness_model.keras"
- "results.csv"
- "README.md"

---

🚀 How to Run the Project

1. Install required libraries:

pip install tensorflow opencv-python matplotlib numpy seaborn scikit-learn

2. Run Jupyter Notebook:

jupyter notebook

3. Open the project file and execute all cells

---

📈 Results

- Achieved ~90% training accuracy
- Successfully classified 4 driver states
- Converted predictions into fatigue levels

---

🧾 Conclusion

- Built a deep learning model using MobileNetV2
- Successfully detected driver drowsiness levels
- Model can classify eye and yawning states effectively
- Can be extended to real-time driver monitoring systems

---

🔮 Future Scope

- Real-time webcam detection using OpenCV
- Alert system (sound alarm)
- Mobile app integration
- Deployment using Streamlit

---

👩‍💻 Author

Mohana Selvi
