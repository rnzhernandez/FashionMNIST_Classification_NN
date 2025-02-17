# FashionMNIST_Classification_NN
This repository contains an implementation of neural network models for classifying fashion images using the Fashion MNIST dataset. The project focuses on training and evaluating different neural network architectures to understand the impact of various hyperparameters, network structures, and optimisers on model performance. The implementation is done using Python with TensorFlow/Keras.

## Process
The dataset is preprocessed by normalising pixel values, reshaping images for CNN input, and converting labels to one-hot encoding. Three key tasks are performed:

- **Fully Connected Neural Network (Dense Layers Only)** – A baseline dense model is built, and its performance is optimised by adjusting the number of layers, neurons, and activation functions.
- **Convolutional Neural Network (CNN)** – CNN models are implemented to extract spatial features, experimenting with convolutional layers, filter sizes, pooling layers, and activation functions.
- **Optimiser and Learning Rate Tuning** – The best CNN model is selected, and different optimisers (SGD, Adam, RMSprop) and learning rates are tested to improve accuracy.

## Key Insights
- **Dense vs. CNN:** CNN models significantly outperform fully connected networks by capturing spatial hierarchies in images.
- **Architecture Impact:** Increasing the number of layers and filters improves performance up to a point, but excessive complexity leads to overfitting.
- **Optimization Strategies:** Adam consistently provides better convergence than SGD, though fine-tuning learning rates affects stability and final accuracy.
- **Trade-offs:** Higher model complexity improves accuracy but increases training time. Regularisation techniques (dropout, batch normalisation) help balance performance.

Models are evaluated based on accuracy, and performance is ranked. The report includes architecture details, optimiser choices, experiment results, and key findings. The code is structured for clarity and reproducibility, ensuring insights can be effectively applied to similar classification tasks.
