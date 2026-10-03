# DAY--12

# Light Level TFLite Classifier

## Project Description

This project demonstrates a TensorFlow neural network that classifies light-level readings into three categories:

- Dark
- Normal
- Bright

The trained model is converted into TensorFlow Lite format and tested using Python.

## Objective

To train a small TensorFlow model, convert it into a `.tflite` file, and verify that the TFLite model produces the same output as the original TensorFlow model.

## Technologies Used

- Python
- TensorFlow
- NumPy
- TensorFlow Lite
- Google Colab

## Light-Level Categories

| Light Level | Category |
|-------------|----------|
| 0 – 300 | Dark |
| 301 – 700 | Normal |
| 701 – 1000 | Bright |

## Model

A simple neural network with Dense layers and Softmax activation is used.

- Optimizer: Adam
- Loss Function: Sparse Categorical Crossentropy
- Epochs: 500

## Test Values

The model is tested using:

- 150 → Dark
- 500 → Normal
- 900 → Bright

## TFLite Conversion

The trained TensorFlow model is converted into a TensorFlow Lite model.

Generated file:

`light_classifier.tflite`

## Result

The TFLite model successfully performs inference and produces the same classification results as the original TensorFlow model.

## Files

- `light_level_classifier.ipynb` – Complete Google Colab notebook
- `light_classifier.tflite` – Converted TensorFlow Lite model
- `README.md` – Project documentation

## Platform

Google Colab
