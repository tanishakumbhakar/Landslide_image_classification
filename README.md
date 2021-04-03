# Landslide image classification using pretrained CNN models with fine-tuning and image augmentation
The aim of this project is to use different pre-trained transfer learning models for classification of images containing landslides and compare them.<br>
Dataset used consists of total 500 images of landslide downloaded from google.<br>
The training dataset consists of 400 images (80 % of total dataset), validation dataset consists of 50 images (10 % of total dataset), test dataset consists of 50 images (10 % of total dataset).
## Steps:
1. Sample image is first pre-processed which consists of 4 steps: Image resizing, Image scaling, Label encoding (Landslide - 0, others - 1) and Image augmentation<br>
2. The pre-trained models (VGG-16, VGG-19, ResNet101) are fine-tuned to build the last classifier. <br>
3. Then, the model is trained for 100 epochs.
4. Three different pre-trained models of VGG-16, VGG-19, ResNet-101 are evaluated by first testing them on a sample test image, then visualizing how a CNN model actually tries to analyze and extract
features from the image, and finally by testing each model's performance on our test dataset.
## Results:
### VGG-16 model pre-trained on imagenet weights:
Accuracy: 0.4 <br>
Precision: 0.4762<br>
Recall: 0.4<br>
F1 Score: 0.4348<br>

### VGG-19 model pre-trained on imagenet weights:
Accuracy: 0.32 <br>
Precision: 0.5<br>
Recall: 0.32<br>
F1 Score: 0.3902<br>

### ResNet-101 model pre-trained on imagenet weights:
Accuracy: 0.42 <br>
Precision: 0.5<br>
Recall: 0.42<br>
F1 Score: 0.4565<br>
