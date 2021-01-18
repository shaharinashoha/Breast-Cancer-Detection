# Breast-Cancer-Detection
Classify cancerous images (IDC : invasive ductal carcinoma) vs non-IDC images.

The dataset consists of 5547 breast histology images each of pixel size 50 x 50 x 3. The goal is to classify cancerous images (IDC : invasive ductal carcinoma) vs non-IDC images. In a first step we analyze the images and look at the distribution of the pixel intensities. Then, the images are normalized and we try out some basic classification algorithms like logistic regression, random forest, decision tree and so on. We validate and compare each of these base models. After that we implement the following neural network architecture:

input layer: [., 50, 50, 3]

layer: Conv1 -> ReLu -> MaxPool: [., 25, 25, 36]

layer: Conv2 -> ReLu -> MaxPool: [., 13, 13, 36]

layer: Conv3 -> ReLu -> MaxPool: [., 7, 7, 36]

layer: FC -> ReLu: [., 576]

output layer: FC -> ReLu: [., 2]
