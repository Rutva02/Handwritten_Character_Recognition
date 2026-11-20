# Handwritten Character Recognition using CNN

## Project Overview
This project uses a Convolutional Neural Network (CNN) to recognize handwritten digits (0–9) from images. The model is trained and tested using the MNIST handwritten digit dataset.

## Dataset
- Dataset: MNIST
- Total images: 70,000
- Training images: 60,000
- Testing images: 10,000
- Image size: 28 × 28 pixels
- Number of classes: 10 (digits 0–9)

## Technologies Used
- Python
- TensorFlow and Keras
- NumPy
- Matplotlib
- Scikit-learn
- Seaborn
- Google Colab

## Model Architecture
The CNN model consists of:
- Two Convolutional layers
- Two Max Pooling layers
- Flatten layer
- Dense layer with ReLU activation
- Dropout layer
- Output layer with Softmax activation

## Project Workflow
1. Imported required libraries.
2. Loaded the MNIST dataset.
3. Visualized sample handwritten digits.
4. Normalized and reshaped the images.
5. Built the CNN model.
6. Compiled and trained the model.
7. Evaluated model performance.
8. Generated digit predictions.
9. Created a classification report and confusion matrix.
10. Saved the trained model.

## Model Training
- Epochs: 5
- Batch Size: 64
- Optimizer: Adam
- Loss Function: Sparse Categorical Crossentropy
- Validation Split: 10%

## Results

| Metric | Result |
|---|---:|
| Training Accuracy | 98.62% |
| Validation Accuracy | 99.10% |
| Test Accuracy | 99.14% |
| Test Loss | 0.0271 |

## Project Files
- `Handwritten_Character_Recognition.ipynb` – Complete source code, training, evaluation, and visualizations.
- `handwritten_digit_model.keras` – Saved trained CNN model.

## How to Run
1. Download the Jupyter Notebook.
2. Open it using Google Colab.
3. Run the notebook cells in sequence.
4. The MNIST dataset will be loaded automatically through TensorFlow/Keras.
5. Train the CNN and evaluate its performance.

To load the saved model:

```python
from tensorflow.keras.models import load_model

model = load_model('handwritten_digit_model.keras')
```

## Conclusion
The CNN model successfully recognizes handwritten digits and achieved 99.14% accuracy on the MNIST test dataset. This project demonstrates the application of deep learning and CNNs in image classification.

