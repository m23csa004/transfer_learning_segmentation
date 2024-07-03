Overview
This project uses a skin lesion classification model using a pre-trained MobileNet encoder and a custom decoder. The model is trained and tested on the ISIC 2016 dataset of skin lesion images and corresponding masks. The goal is to accurately classify the lesion areas in the images.

Program Schedule
Creating data structures:

The data structure is loaded and manipulated using the PyTorch Dataset and DataLoader classes.
Data enhancement techniques such as magnification, horizontal and vertical flipping, and color jittering are applied to the training images.

Good building materials:

The pre-trained MobileNetV2 is used as an encoder.
A custom decoder is designed to upsample the output of the encoder to match the input image size.
The model is designed for binary segmentation with one output channel representing the lesion mask.

Training and Certification:

The model is trained using Binary Cross Entropy with Logits Loss function.
The ADAM optimizer is used with a learning rate of 0.001.
Training and certification losses are tracked and mapped for analysis.

Evaluation metrics:

Classification performance is evaluated using Intersection over Union (IoU) and Dice Score.
After analysis, IoU and average Dice Score are reported.

outputs:

Exemplary images, ground truth masks, and predicted masks are presented to verify the performance of the model.