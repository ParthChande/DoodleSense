# DoodleSense
DoodleSense is a machine learning project that trains a convolutional neural network to classify doodles and provides a GUI for real-time predictions. Leveraging the Quick, Draw! dataset, it offers an interactive tool to explore AI's ability to recognize hand-drawn sketches with high accuracy.

# Key Features
- Automated Data Downloading: Automatically download and preprocess doodle datasets from the Quick, Draw! dataset.
- Efficient Data Loading: Utilize TensorFlow's GPU capabilities for fast data loading, reshaping, and normalization.
- Data Augmentation: Enhance the training data with various augmentation techniques to improve model generalization.
- Model Training: Train a deep CNN with mixed precision to efficiently learn and classify multiple categories of doodles.
- Interactive GUI: Provide a user-friendly interface to draw doodles and get real-time predictions from the trained model.
- High Accuracy: Achieve high accuracy in classifying doodles through a well-architected CNN and advanced training techniques.

# CNN
The SketchSense project employs a deep convolutional neural network (CNN) designed to classify hand-drawn doodles from the Quick, Draw! dataset. Here are the key details about the CNN architecture:

**Layers:**
- Convolutional Layers: The CNN consists of multiple convolutional layers with 3x3 filter kernels, employing 'relu' activation functions to extract features from input images.

- MaxPooling Layers: MaxPooling layers with 2x2 pooling windows are used to downsample the feature maps and reduce computational complexity.

- Dropout Layers: Dropout layers are added after each convolutional block to prevent overfitting by randomly setting a fraction of input units to zero during training.

- Dense Layers: Fully connected dense layers are employed towards the end of the network to perform classification based on extracted features.

**Training Strategy:**
- Optimizer: The model is optimized using the Adam optimizer, which adapts learning rates for each parameter.

- Loss Function: Categorical crossentropy loss is utilized as the loss function for multi-class classification tasks.

- Metrics: Model performance is evaluated using accuracy metrics to measure the percentage of correctly classified doodles.

**Special Techniques:**
- Data Augmentation: Training data is augmented using techniques such as rotation, zooming, shifting, and flipping to enhance model generalization.

- Mixed Precision Training: Mixed precision training is enabled using TensorFlow's capabilities to leverage float16 computations for faster and more memory-efficient training on compatible hardware.

**Deployment:**
- The trained CNN model is deployed within an interactive GUI application, enabling users to draw doodles and receive real-time predictions, showcasing the CNN's effectiveness in recognizing diverse doodle categories.

# Model Summary
![image](https://github.com/ParthChande/DoodleSense/assets/119730313/483c10a3-1849-4317-a040-51e316bd3af3)

![image](https://github.com/ParthChande/DoodleSense/assets/119730313/5ebd54d5-878d-41ee-8fc7-14a2b9eea5e2)

# Predictor
![image](https://github.com/ParthChande/DoodleSense/assets/119730313/e9e75c7a-dfd5-4ca7-8361-909ee85cccdd) ![image](https://github.com/ParthChande/DoodleSense/assets/119730313/47823082-9ab9-4841-9e45-c678acbdcb67)


