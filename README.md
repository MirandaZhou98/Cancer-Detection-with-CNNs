# Cancer-Detection-with-CNNs
Detection of Cancer in pathology images of breast tissues using deep learning

## Motivation:
The goal of this project is to assist pathologists in detecting cancer cells in gigapixel pathology images. Visual inspection of the pathology slides is error prone and tedious for the already rare expertise. Hence, we hope to provide assistance in these detections for the doctors.

## Data:
Gigapixel pathology slides. There are multiple different zoom levels for each slide
https://camelyon17.grand-challenge.org/Data/

## Method:
To simplify the image analysis, I tackle the issue as a binary classification problem. I seperate the slide into many small grids and determine whether or not there is tumorous cells within that grid. I then color those grids based on my prediction to create a heat map for the pathologist to see. I utilized the Inception(V3) Architecture for transfer learning.

I had 2 approaches
* Single Zoom Level: On zoom level 2. Single CNN.
* Dual Zoom Level: On zoom level 2 and 3. Take in 2 inputs of different zoom levels centered at the same location to make the prediction

## Google Colab Notebook:
Single-zoom: https://colab.research.google.com/drive/1Ce5wZIhNJr53mmaNAIYWj5FV5Bn3hJEQ?usp=sharing
Multi-zoom: https://drive.google.com/file/d/1FkqDyuX5bnrCoUYuIPe1UTpnNZbkihf5/view?usp=sharing

