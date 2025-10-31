Project title : Handwritten Word Recognition
This project implements a deep learning-based handwritten word recognition system using multiple neural architectures(like CNN,CNN-LSTM,CNN-GRU and Transfer
learning models such as VGG16,ResNet50V2 and EfficientNetB0).

Dataset used: IAM Handwritten Forms Dataset from Kaggle 

Before starting the project,install all the required libraries and dependencies:
Use:  !pip install kagglehub scikit-learn tensorflow
and upload your Kaggle API token(kaggle.json file downloaded from kaggle)

Steps:
1. Automated dataset download from Kaggle
2. Image preprocessing and label extraction from XML metadata
3. Implementation of all the six models 
4. Model training,validation and performance comparison
5. Visualization of confusion matrices and classification reports
6. Automatic selection of the best-performing model

Model Architectures:
1. CNN Classifier -> Standard convolutional neural network for image classification
2. CNN-LSTM       -> CNN feature extractor+Bidirectional LSTM for sequence modeling
3. CNN-GRU	      -> CNN feature extractor+Bidirectional GRU for temporal understanding
4. VGG16, ResNet50V2, EfficientNetB0 -> Transfer learning pre-trained models

Technologies Used:
1. Python,TensorFlow/Keras,OpenCV,NumPy,Matplotlib,scikit-learn
2. Google Colab for cloud-based training
3. KaggleHub for dataset management

Configurations:
1. Input Image Size(Grayscale) -> 64 × 256 × 1
2. Input Image Size(for Transfer Models)	-> 64 × 256 × 3
3. Max Samples ->	10000
4. Top K Words(Classes) -> 20
5. Batch Size -> 32
6. Epochs(for all models)	-> 100
   
Accuracy -> 74.53%
Training Set = 80% -> 8000samples
Testing Set = 20% -> 2000samples

Analysis:
MAX_SAMPLES=2000,EPOCHS=6 -> Accuracy = 42.86%
MAX_SAMPLES=2000,EPOCHS=20 -> Accuracy = 60.87%
MAX_SAMPLES=2000,EPOCHS=50 -> Accuracy = 69.57%
MAX_SAMPLES=2000,EPOCHS=80 -> Accuracy = 70.19%
MAX_SAMPLES=10000,EPOCHS=6 -> Accuracy = 42.86%
MAX_SAMPLES=10000,EPOCHS=20 -> Accuracy = 60.87%
MAX_SAMPLES=10000,EPOCHS=50 -> Accuracy = 69.57%
MAX_SAMPLES=10000,EPOCHS=100 -> Accuracy = 74.53%
MAX_SAMPLES=10000,EPOCHS=300 -> Accuracy = 75.78%
MAX_SAMPLES=13000,EPOCHS=50 -> Accuracy = 69.57%
MAX_SAMPLES=15000,EPOCHS=50 -> Accuracy = 70.81%
