## Machine learning in Matlab

 - Training a network from scratch.
 - Using transfer learning to train on existing network.
 - Training an existing network to perform semantic segmentation.
**In this text we consider these logics for image classification.**

The neural networks which are available in Matlab are as following:

 - LeNet
 - GoogleNet (4)
 - Tensorflow
 - Keras 
 - Yolo 
 - SSD 
 - ResNet
 - AlexNet (1)
 - ResNet
 - VGG 16/19 (2,3)


For using each of them only three four lines are neccessary.

### Training a model from scratch

For developing a model we can use Convolutional neural network (CNN) and we can identify handwritting when a person write a digit.
The second thing that we need is the data, the models use data to learn some thing. More data precizer is the model. One possibility is MNIST dataset.

```mermaid
graph LR
A[Access Data] --> B[Configure Network Layers]
B--> C[Train Network]
C--> D[Check Accuracy]
D--> E[Done]
```
**Accessing the data**

With the folowing code we can download the binary file, which contains images and read the images into array.

```matlab
rawImgDataTrain = uint8(fread(fid, numImg * numRows * numCols,...'uint8'));
% Reshape the data part into a 4D array
rawImgDataTrain = reshape(rawImgDataTrain, [numRows, numCols,...numImgs]);
imgDataTrain(:,:,1,ii) = uint8(rawImgDataTrain(:,:,ii));
```
**Creting and Configuring networks layers**

The convolutional network is the common type of deep learning network. It contains different layers. With each layer the
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTgzNjU5NjExNywtMTUzMjQ2NzE4OSwtMT
ExODcwNTYwNywtNDYzMjg2NzgsLTQ2MzI4Njc4LC0yMTU5OTU1
MzQsLTEzNDk4NDUyMjYsMTg1NDkwMjksMTkwMTk5MDc1M119
-->