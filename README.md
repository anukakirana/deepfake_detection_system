# deepfake_detection_system
Deepfake Image detection project with a 3-layer CNN model, locally hosted for real-time image classification via a web interface.
# Deepfake Image Detection System

This is a locally run deepfake image detection system that uses a custom Convolutional Neural Network (CNN) to classify images as either real or deepfake. The model is accessed through a simple web interface using HTML, CSS, and JavaScript, while the backend logic is implemented in Python.

---

## Workflow

### Step 1: Image Upload
Users upload an image through the local HTML interface. The image can be either authentic or manipulated (deepfake).

### Step 2: Image Preprocessing
The uploaded image is processed using OpenCV. It is resized to 224x224 pixels, normalized, and converted to the format required by the CNN model.

### Step 3: Model Prediction
The preprocessed image is passed to the trained CNN model for binary classification.

### Step 4: Result Display
Based on the prediction output, the user is informed whether the uploaded image is real or a deepfake.

---

## CNN Architecture

- **Input Layer**: 224x224x3 RGB image  
- **Convolutional Layer 1**: 32 filters, ReLU activation, followed by 2x2 MaxPooling  
- **Convolutional Layer 2**: 64 filters, ReLU activation, followed by 2x2 MaxPooling  
- **Convolutional Layer 3**: 128 filters, ReLU activation, followed by 2x2 MaxPooling  
- **Flatten Layer**  
- **Dense Layer**: 512 neurons, ReLU activation  
- **Output Layer**: 1 neuron with Sigmoid activation (for binary classification)

---

## Technologies Used

- Python  
- TensorFlow / Keras  
- OpenCV  
- HTML, CSS, JavaScript (for the frontend interface)  

---

## How to Run Locally

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/deepfake_detection_system.git
   cd deepfake_detection_system
