
# 🦠 Malaria Cell Image Classification

This repository presents a machine learning pipeline for classifying parasitized and uninfected cells using the NIH Malaria Dataset. It includes a custom convolutional neural network (LightCNN) as a proposed model, and a baseline implementation using transfer learning with MobileNetV2.

## 📁 Repository Structure

```
├── cell_images/                    # Full NIH malaria cell dataset
├── saved_model/                   # Trained model checkpoints
├── statistics/                    # Model evaluation reports & plots
├── tuned_models/                  # Fine-tuned versions of models
├── malaria_detection_tuned.ipynb  # Custom CNN (LightCNN) with hyperparameter tuning
├── malaria_transfer_learning.ipynb# MobileNetV2-based transfer learning implementation
├── model_statistics.ipynb         # Visualization & statistical performance analysis
├── LICENSE
└── .gitignore
```

## 🎯 Project Objective

To develop an accurate image classification model that distinguishes between parasitized and uninfected blood cells using deep learning. The project explores:

- A **custom lightweight CNN (LightCNN)** designed and tuned from scratch.
- **Transfer learning** using a pretrained **MobileNetV2** model for a baseline comparison.
- **Hyperparameter tuning** with Keras Tuner.
- **Model evaluation** using key metrics such as accuracy, precision, recall, F1-score, and confusion matrices.

## 🧪 Dataset

The [NIH Malaria Dataset](https://lhncbc.nlm.nih.gov/publication/pub9932) contains 27,558 segmented cell images (13,779 parasitized and 13,779 uninfected). All images are of equal dimensions (typically 128x128 pixels).

## ⚙️ Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/malaria-cell-classification.git
   cd malaria-cell-classification
   ```

2. **Install dependencies**:
   Ensure you have Python 3.7+ and install packages via pip:
   ```bash
   pip install tensorflow keras keras-tuner keras-applications
   ```

3. **Run Notebooks**:
   Launch the following notebooks to explore the workflow:
   - `malaria_transfer_learning.ipynb`: Transfer learning with MobileNetV2
   - `malaria_detection_tuned.ipynb`: Custom LightCNN with hyperparameter tuning
   - `model_statistics.ipynb`: Performance analysis and visualization

## 📊 Results & Evaluation

- Custom LightCNN showed improved performance after tuning.
- MobileNetV2 serves as a strong baseline but was outperformed by the proposed model in some metrics.
- Detailed plots and metrics can be found in the `statistics/` folder and the `model_statistics.ipynb` notebook.

## 🛠️ Tech Stack

- **TensorFlow**
- **Keras**
- **Keras Tuner**
- **Keras Applications**
- **Jupyter Notebooks**

## 📄 License

This project is licensed under the [MIT License](LICENSE).
