# APTOS-2019-Blindness-Detection


The challenge was to build a machine learning model to speed up disease detection. You’ll work with thousands of images collected in rural areas to help identify diabetic retinopathy automatically. If successful, you will not only help to prevent lifelong blindness, but these models may be used to detect other sorts of diseases in the future, like glaucoma and macular degeneration.

My complete workflow for the APTOS 2019 competition:

1. Loading & Exploration: A quick overview of the dataset
2. Resize Images: We will resize both the training and test images to 224x224 so that it matches the ImageNet format.
3. Mixup & Data Generator: We show how to create a data generator that will perform a random transformation to our datasets (flip vertically/horizontally, rotation, zooming). This will help our model generalize better to the data since it is fairly small (only ~3000 images).
4. Quadratic Weighted Kappa: A thorough overview of the metric used for this competition, with an intuitive example. Check it out!
5. Model: We will use a DenseNet-121 pre-trained on ImageNet. We will finetune it using Adam for 15 epochs, and evaluate it on an unseen validation set.
6. Training & Evaluation: We take a look at the change in loss and QWK score through the epochs.

Better Results:
1. More training can increase the accuracy although 60 epochs give an accuracy of 86%
2. Parameter Tuning can significantly give you an edge over the accuracy.

In Top 46% ( 1330 in 3000 teams) at https://www.kaggle.com/satyamsharma
