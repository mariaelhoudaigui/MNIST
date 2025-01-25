# MNIST Project: Handwritten Digit Classification

This project uses a Convolutional Neural Network (CNN) model to classify handwritten digits from the MNIST dataset. 
It includes data preparation, model training, evaluation, and testing using a user-friendly interface with Gradio.

## Features

- *Handwritten Digit Classification*: Classify handwritten digits (0-9) in static images, displaying the predicted digit.
- *Model Evaluation*: Evaluate the trained model’s accuracy and performance on a test dataset.
- *Visualization of Results*: Visualize detection results directly on the interface with the predicted digit displayed.
- *User Interface*: Use Gradio to provide an intuitive interface for users to upload images and get predictions.

---

## Technologies Used

- *MNIST Dataset*: The dataset used for training the model, consisting of 70,000 28x28 grayscale images of handwritten digits.
- *TensorFlow/Keras*: Used to create, train, and evaluate the CNN model for digit classification.
- *Gradio*: A Python library used to build the user interface for the application.
- *Matplotlib*: Used for plotting and visualizing results during model training and evaluation.

## **Model Saving and Loading**

After training the model, it is saved using the `model.save()` function, which stores the best-performing model weights in a file. This allows you to use the model for inference or testing later without retraining it.

### **Saving the Model:**

Once the model is trained, save it using the following code:

```python
# Save the model after training
model.save("/content/bestmodel.keras")
