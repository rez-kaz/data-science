# Assignment 4 - Foundations of Data Science

This project is the implementation of Assignment 4 for the Foundations of Data Science course.

It covers several stages of the workflow, from data cleaning and preprocessing to modeling, evaluation, and interpretation.

The goal was to keep the work practical and connected, so the notebook feels like one continuous pipeline instead of separate isolated tasks.

## Author
**Reza Kazemini Moghadam**

## Datasets Used

### 1) Bank Marketing
The main file for this part is `bank-full.csv`.

This dataset is used for a binary classification task.

The goal is to predict whether a customer will respond to a marketing campaign.

In this section, the raw data was first inspected and cleaned, then prepared for modeling.

### 2) MNIST
MNIST is used in multiple parts of the notebook.

It contains handwritten digit images.

I used it to explore generative models and explainable AI.

It is a simple dataset, but it works very well for showing how these models behave visually.

### 3) Mammogram Dataset
This dataset is used in the bonus and final pipeline section.

Dataset source: https://data.mendeley.com/datasets/fvjhtskg93/1

It contains breast cancer images with classes such as `Cancer` and `Non-Cancer`.

Because the dataset is imbalanced, balancing techniques were used during training.

## Assignment Structure

This assignment includes **7 parts**.

The first six parts are implemented on different datasets with different goals.

The seventh part is a full end-to-end pipeline on a single dataset.

In Part 7, the ideas from the earlier parts are reused on the mammogram dataset.

## Main Parts

1. Bank Marketing data loading, cleaning, and initial preparation
2. Modeling on the imbalanced Bank Marketing dataset
3. `VAE` on MNIST
4. `GAN` on MNIST
5. `Diffusion` on MNIST
6. `XAI` and `Grad-CAM` on MNIST
7. Full pipeline on the mammogram dataset

## Models and Methods

The notebook includes the following models and methods:

- `SimpleCNN`
- `VAE`
- `GAN`
- `Diffusion`
- `Grad-CAM`

For the mammogram section, I also used training-data balancing and synthetic augmentation.

## Final Pipeline

The final pipeline follows a simple and clear flow:

- load the data
- clean and prepare it
- split it into train and test sets
- balance the training set
- add synthetic samples when needed
- train the model
- evaluate the final results

This makes Part 7 a complete practical workflow rather than just a small experiment.

## Important Note

For the mammogram task, accuracy alone is not enough.

Since the positive class is the minority class, recall and F1-score are more important.

That is why balancing the data was an important part of the training process.

## Files

- `Assignment4.ipynb`
- `bank-full.csv`
- `ADS 2026 - Assignment 4-1.pdf`
- `Mammogram Mastery A Robust Dataset for Breast Cancer Detection and Medical Education`

## Summary

This assignment shows a full journey from raw data to model output.

It starts with a tabular binary classification problem.

Then it moves to image-based generative modeling on MNIST.

Finally, it ends with a medical imaging pipeline on the mammogram dataset.

The notebook combines classic machine learning, deep learning, generative modeling, and explainable AI in one project.


