## 📄 Project Overview
This project uses a **Convolutional Neural Network (CNN)** to classify traffic signs from the **German Traffic Sign Recognition Benchmark (GTSRB)** dataset. The model recognizes **43 different traffic sign classes**, essential for autonomous driving and driver assistance systems.

## 🔑 Key Features
- **Data Preprocessing:**  
  - Images resized to **32×32 pixels** and normalized (0–1 scale).  
  - Labels one-hot encoded for multi-class classification.  

- **CNN Architecture:**  
  - Three convolutional layers (filters: 32, 64, 128) with **ReLU activation**.  
  - **MaxPooling** after each convolutional layer.  
  - **Dropout layers** (0.5 after conv layers, 0.6 in dense layer) to reduce overfitting.  
  - Fully connected layers with **128 units** and **softmax output** for 43 classes.  

- **Training:**  
  - **30 epochs** using **Adam optimizer** and **categorical cross-entropy loss**.  

- **Performance:**  
  - Achieves over **98% validation accuracy**, showing strong generalization.  

## 🗂 Dataset
- **Total images:** 51,839 (32×32×3)  
- **Split:**  
  - Training: 34,799  
  - Validation: 4,410  
  - Testing: 12,630  
- **Classes:** 43 (speed limits, warning, directional, and prohibitory signs).  

## 📊 Results
- **Training Accuracy:** ~98.5%  
- **Validation Accuracy:** ~98.1%  
- Stable validation loss indicating no significant overfitting.  

## 🚀 Applications
- Autonomous vehicle systems  
- Driver assistance tools  
- Traffic monitoring  
- Road safety applications  

## 🛠 Technologies Used
- **Python**, **TensorFlow/Keras**  
- **OpenCV** for image processing  
- **Pandas**, **NumPy** for data handling  
- **Matplotlib** for visualization  
