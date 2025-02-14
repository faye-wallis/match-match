# Match-Match
## Image Classification with Style

This project utilizes a convolutional neural network to classify clothing images based on type.
Our model was trained on the popular Fashion MNIST dataset, which contains 80,000 clothing images saved as 28x28 pixel arrays.
Match-Match integrates this training data and processes it through 5 layers - Conv2D, MaxPooling, Flatten, Dropout, and a Dense layer with the softmax activation function.
These layers work together to recognize the distinct features of each 2D array, process them into a format readable to the output layer, and then produce an accurate classification.

The accuracy of Match-Match predictions are verified by plotting each set of images against the confidence array produced by the softmax output layer.
The prediction with the highest confidence value is shown side by side with the actual class of the given image, allowing users to follow the "thought process" of the model, even when incorrect.

After two iterations of the model which were not as well suited to 2D image processing, this final version of Match-Match is able to classify clothing items with 90% accuracy.
Once the model is trained, users can input new images by passing them through our MNISTIFY function, which reduces any image into a grayscaled 28x28 array just like the Fashion MNIST dataset.
