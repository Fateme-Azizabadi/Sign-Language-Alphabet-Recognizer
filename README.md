# Sign Language Alphabet Recognizer

**This Project aims to use MLP Architecture to classify the Sign Language Dataset.**

* Test and training Data can be found in the Dataset File. 80% of training data is allocated to training data and 20% to validation data.

The image below shows some of the first 25 images with their labels.

![](https://github.com/Fateme-Azizabadi/Sign-Language-Alphabet-Recognizer/blob/main/Images/Dataset.png)

* MLP Classifier is used to classify sign language data. None of the ready-made libraries were used to create this classifier, and this model was implemented from scratch.

* Five layers have been considered for this classifier. (3 hidden layers and one output layer)

* Since the input data contains 783 pixels (28 x 28), the number of input neurons is 783. The first to fifth hidden layers contain 392 neurons, and the last layer has 39 neurons. (39 outgoing classes.)

* A function is written as neural-network that makes the MLP network of this classifier.

* The learning rate is 0.001, and the batch size is 128.

* After preparation, the data enters the Next-Batch function, where the data based on the Size Batch are separated, and Shuffle is applied to them. Then the data are entered into the neural network to determine their weights.

* Two Optimizers (ADAM and SGD) are used in this training.

* Batch Normalization and dropout also are used to improve the performance and reduce the overfitting problem. 

* Also, up-sampling/down-sampling and SMOTE technics are used to solve the unbalanced dataset problem. 

* Ultimately, we used WebCam to test the network in real life. 


