## Artificial Neural Network (ANN)

### Basics
A simple neural network consists of input units, weighted connections, and an output unit. Each unit computes a weighted sum of inputs, adds a bias, and applies an activation function (e.g., step, sigmoid, Rectified linear unit - ReLU) to determine the output.

![Simple_neural_network](assets/SimpleNeuralNet.png)

### Training Basic Neural Network
**Gradient Descent:** Used to minimize loss by iteratively adjusting weights. It calculates the gradient (direction to reduce loss) based on all data points, updates weights, and repeats. Computationally expensive due to processing all data points.

**Limitation of Single Layer Neural Network:**
One simple layer of input and one layer of output might be useful for classification binary output (linear decision boundary). It doesnt work for complex output where data cant be linearly separable. This is when the multi-layer neural network come into play.

### Multilayer Neural Networks 
Include input, hidden, and output layers. Hidden layers allow modeling of complex, non-linearly separable functions (e.g., distinguishing points not separable by a single line).

### Training Multilayer Neural Network
**Backpropagation:** Trains multilayer networks by calculating output layer error, propagating it backward to update weights in hidden layers, using calculus to estimate errors.

**Deep Neural Networks:** Neural network with multiple hidden layers.

**Overfitting:** Overfitting in machine learning occurs when a model learns the training data too well, including its noise and irrelevant details, resulting in poor performance on new, unseen data. Essentially, the model becomes overly tailored to the training set and loses its ability to generalize to new, different data. The solution for this is to Dropout.

**Dropout:** Randomly removes units during training to prevent over-reliance on specific nodes, enhancing robustness of the model.

### Example Implementation of Neural Network: TensorFlow
It applies all the concepts above. Playground: https://playground.tensorflow.org/

**N.B.** In machine learning, both regression and classification are supervised learning techniques used for different prediction tasks. Regression predicts continuous numerical values, while classification predicts categorical labels. Essentially, regression deals with "how much" or "how many", while classification deals with "what kind" or "which category". 
