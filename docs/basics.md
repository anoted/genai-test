[⬅ Back to Main](../readme.md)

## Deep Learning Basics

Deep learning is a subset of machine learning that utilizes neural networks with multiple layers to model complex patterns in data. It has been successfully applied to various domains, including computer vision, natural language processing, and bioinformatics.

### Neural Networks
A neural network consists of layers of neurons that transform input data through weighted connections. The main components of a neural network include:

- **Input Layer**: Receives input features.
- **Hidden Layers**: Perform computations and feature extraction.
- **Output Layer**: Produces the final prediction or classification.

#### Activation Functions
Activation functions introduce non-linearity to the model, enabling it to learn complex patterns. Common activation functions include:

- **Sigmoid**: $f(x) = \frac{1}{1 + e^{-x}}$
- **ReLU (Rectified Linear Unit)**: $f(x) = \max(0, x)$
- **Tanh**: $f(x) = \frac{e^x - e^{-x}}{e^x + e^{-x}}$
- **Softmax**: Used for multi-class classification

### Training a Neural Network
Neural networks are trained using optimization techniques that minimize a loss function. The main steps in training include:

1. **Forward Propagation**: Compute predictions by passing input through the network.
2. **Loss Calculation**: Measure the error using a loss function (e.g., Mean Squared Error, Cross-Entropy Loss).
3. **Backward Propagation**: Compute gradients using backpropagation.
4. **Weight Update**: Adjust weights using an optimizer (e.g., Stochastic Gradient Descent, Adam).

### Optimization Algorithms
Optimization algorithms improve training efficiency. Common optimizers include:

- **SGD (Stochastic Gradient Descent)**
- **Adam (Adaptive Moment Estimation)**
- **RMSprop (Root Mean Square Propagation)**

### Regularization Techniques
Regularization prevents overfitting by introducing constraints on the model. Popular techniques include:

- **Dropout**: Randomly deactivates neurons during training.
- **L1 and L2 Regularization**: Adds penalty terms to the loss function.
- **Batch Normalization**: Normalizes activations to stabilize training.

### Deep Learning Architectures
Different architectures are designed for specific tasks:

- **Convolutional Neural Networks (CNNs)**: Used for image processing.
- **Recurrent Neural Networks (RNNs)**: Handles sequential data like time series and text.
- **Transformers**: Used in NLP tasks (e.g., BERT, GPT).
- **Autoencoders**: Used for dimensionality reduction and anomaly detection.

## Frameworks and Libraries
Popular deep learning frameworks include:

- **TensorFlow**
- **PyTorch**
- **Keras**

[⬅ Back to Main](../readme.md)