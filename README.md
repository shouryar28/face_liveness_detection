# face_liveness_detection
Data Preparation: Converted BioID Face Database images from .pgm to .jpg format using OpenCV, organized them into training and validation sets, and applied image augmentation.

Model Architecture: Built a CNN using TensorFlow and Keras with Conv2D and MaxPooling2D layers, followed by Dense layers for binary classification to detect real vs. fake faces.

Training & Validation: Trained the model using ImageDataGenerator with 80-20 train-validation split, implementing EarlyStopping to avoid overfitting.

Real-Time Detection: Integrated OpenCV for real-time face detection from webcam feed, using Haar cascades to preprocess faces and the trained model to predict liveness.

Deployment: Implemented a live system that labels detected faces as "Real" or "Fake" based on model predictions, and displayed bounding boxes on the video feed.
