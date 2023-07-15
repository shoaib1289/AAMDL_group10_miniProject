# Gender Classification using Convolutional Neural Networks

## Model Summary
| Layer (type) | Output Shape | Param # |
| --- | --- | --- |
| conv2d (Conv2D) | (None, 96, 96, 32) | 320 |
| max_pooling2d (MaxPooling2D) | (None, 48, 48, 32) | 0 |
| conv2d_1 (Conv2D) | (None, 48, 48, 32) | 9248 |
| max_pooling2d_1 (MaxPooling2D) | (None, 24, 24, 32) | 0 |
| flatten (Flatten) | (None, 18432) | 0 |
| dense (Dense) | (None, 128) | 2359424 |
| dense_1 (Dense) | (None, 2) | 258 |


## Loss Function
- LaTeX equation for the categorical cross-entropy loss function

The model's loss function is the <span style='color:blue'>**categorical cross-entropy**</span>, which for two classes is computed as:

$$
-\sum_{i=1}^{m} y_i \log(\hat{y}_i)
$$>

Where:
- $y_i$ is the true label
- $\hat{y}_i$ is the predicted label
- $m$ is the number of instances

## Sample Image
![Fingerprint]("https://upload.wikimedia.org/wikipedia/commons/b/bf/Fingerprint_picture.svg")