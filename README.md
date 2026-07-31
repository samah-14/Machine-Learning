# 🐟 Fish Species Classification using Convolutional Neural Networks (CNN)

## 📌 Project Overview

This project focuses on **multiclass fish species classification** using **Deep Learning**. A Convolutional Neural Network (CNN) was developed from scratch using TensorFlow and Keras to automatically identify different fish species from images.

The project demonstrates the complete deep learning pipeline, including dataset preprocessing, model development, training, evaluation, and local deployment.

The dataset contains **11 different fish species**, and the trained CNN model achieved a **test accuracy of approximately 96.39%**. :contentReference[oaicite:0]{index=0} :contentReference[oaicite:1]{index=1}

---

## 🎯 Objectives

- Build a CNN model for multiclass fish image classification.
- Perform image preprocessing and data augmentation.
- Train and evaluate the model on unseen data.
- Visualize model performance using accuracy and loss curves.
- Deploy the trained CNN model locally.

---

## 📂 Dataset

The dataset consists of fish images organized into:

- Training Set
- Validation Set
- Test Set

The dataset contains **11 fish species** with:

| Dataset | Images |
|---------|-------:|
| Training | 6,225 |
| Validation | 1,092 |
| Testing | 3,187 |

Images were resized, normalized, and augmented before training. :contentReference[oaicite:2]{index=2} :contentReference[oaicite:3]{index=3}

---

## 🛠 Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## 🧠 CNN Architecture

The CNN model consists of:

- Input Layer (128 × 128 × 3)
- Data Augmentation Layer
- Conv2D (32 filters)
- MaxPooling2D
- Conv2D (64 filters)
- MaxPooling2D
- Conv2D (128 filters)
- MaxPooling2D
- Flatten Layer
- Dense Layer (128 neurons)
- Dropout (0.5)
- Output Layer (11 Classes with Softmax)

The model was compiled using:

- Optimizer: Adam
- Loss Function: Sparse Categorical Crossentropy
- Metric: Accuracy :contentReference[oaicite:4]{index=4}

---

## 🔄 Data Preprocessing

The preprocessing pipeline includes:

- Image resizing
- Pixel normalization
- Data augmentation
  - Random Flip
  - Random Rotation
  - Random Zoom
- Dataset shuffling
- Caching
- Prefetching for improved training performance :contentReference[oaicite:5]{index=5}

---

## 📈 Model Training

- Epochs: 10
- Batch Size: 32
- Optimizer: Adam

Training and validation accuracy improved consistently over the epochs, indicating effective learning by the CNN model. :contentReference[oaicite:6]{index=6}

---

## 📊 Results

### Test Accuracy

**96.39%**

The model achieved strong classification performance on unseen test data. :contentReference[oaicite:7]{index=7}

Performance visualization includes:

- Training Accuracy
- Validation Accuracy
- Training Loss
- Validation Loss :contentReference[oaicite:8]{index=8}

---

## 💻 Local Deployment

The trained CNN model was successfully deployed locally, enabling fish species prediction without requiring cloud resources.

---

## 🚀 Future Improvements

- Implement Transfer Learning using MobileNetV2.
- Train on more powerful hardware or cloud GPUs.
- Expand the dataset with additional fish species.
- Deploy the application on the web using Streamlit or Flask.
- Optimize the model for real-time inference.

---

## ⚠️ Note

Transfer Learning with **MobileNetV2** was explored during development. However, due to hardware memory limitations, it could not be fully trained on the available system. The implementation remains a planned enhancement for future work. :contentReference[oaicite:9]{index=9}

---

## 📁 Project Structure

```
Fish-Species-Classification/
│
├── Fish_Classification.ipynb
├── final_model.h5
├── README.md
├── images/
├── fish_dataset/
└── requirements.txt
```

---

## 👩‍💻 Author

**Samah Hafeez**

B.Tech Computer Science and Engineering

---

## 📜 License

This project is licensed under the **MIT License**.
