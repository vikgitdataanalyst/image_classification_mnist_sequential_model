# image_classification_mnist_sequential_model

Hello! everyone, welcome to my github profile

Steps Involved:
Data Loading & Preprocessing:

1).Loaded the MNIST dataset using keras.datasets.mnist.

2).Normalized pixel values to the range [0, 1].

3).Reshaped images for compatibility with the model (flattened for Dense layers or expanded with channels for CNN).

4).Converted labels to one-hot encoded format.

Model Building:

1).Used the Sequential API to stack layers linearly.

2).Implemented two model variants:

3).Fully Connected (Dense) Network:

4).Input layer with 784 nodes (28×28)

5).Hidden layers with ReLU activation

6). Output layer with 10 nodes (softmax activation) beacuse it is multi-class classification

CNN-based Model (Optional):

1).Conv2D → MaxPooling → Flatten → Dense

2).Compilation:

3).Optimizer: Adam

4).Loss Function: categorical_crossentropy

Metric: accuracy

Training:

1).Trained the model using model.fit() over several epochs with a validation split.

2).Used batch training for efficient updates.

Evaluation:

1).Evaluated model accuracy using model.evaluate() on test data.

2).Computed and visualized the confusion matrix using Seaborn heatmap.


