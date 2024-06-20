# Simple Neural Network for MNIST using NumPy, Pandas, and Matplotlib

This is a simple implementation of a neural network using NumPy to classify handwritten digits from the MNIST dataset. The network consists of three layers: an input layer, a hidden layer, and an output layer. Pandas is used for data manipulation, and Matplotlib is used for data visualization.

## Dataset

The MNIST dataset is a collection of 70,000 grayscale images of handwritten digits, each with a size of 28x28 pixels. The dataset is divided into a training set of 60,000 images and a test set of 10,000 images. Each image is associated with a label indicating the digit it represents.

## Network Architecture

The neural network architecture consists of the following layers:

1. **Input Layer**: This layer represents the input data, which is a flattened 28x28 image (784 pixels).
2. **Hidden Layer**: This layer contains 128 neurons and applies the ReLU activation function.
3. **Output Layer**: This layer has 10 neurons, one for each digit (0-9), and applies the softmax activation function to produce the final output probabilities.

## Implementation Details

The neural network is implemented using NumPy for numerical operations, Pandas for data manipulation, and Matplotlib for data visualization. The key components are:

1. **Weight Initialization**: The weights are initialized using the Xavier initialization method.
2. **Forward Propagation**: The input data is propagated through the network, and the output probabilities are computed.
3. **Loss Function**: The categorical cross-entropy loss is used as the loss function.
4. **Backward Propagation**: The gradients of the loss function with respect to the weights are computed using backpropagation.
5. **Weight Update**: The weights are updated using the computed gradients and the stochastic gradient descent (SGD) optimizer.

## Usage

1. Ensure that you have the MNIST dataset available.
2. Run the `train.py` script to train the neural network.
3. Once the training is complete, run the `test.py` script to evaluate the performance of the trained model on the test set.
4. Use the provided visualization scripts to analyze the learning process and results.

## Dependencies

- NumPy
- Pandas
- Matplotlib
- MNIST dataset

## Future Improvements

This implementation serves as a basic example of a neural network using NumPy, Pandas, and Matplotlib. Future improvements could include:

- Adding more layers or increasing the number of neurons for better performance.
- Implementing regularization techniques (e.g., dropout) to prevent overfitting.
- Exploring different optimization algorithms (e.g., Adam, RMSProp) for faster convergence.
- Integrating visualization tools to understand the learned features and weights.

## Contributing

Contributions to this project are welcome. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.