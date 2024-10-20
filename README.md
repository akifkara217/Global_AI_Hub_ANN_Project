A project where I worked on introductory level classification, data analysis, model development and evaluation techniques in the fields of deep learning and artificial neural networks (ANN) with a large scale fish dataset.

Dataset: https://www.kaggle.com/datasets/crowww/a-large-scale-fish-dataset

# 1- Required Libraries
First of all, I imported the necessary libraries in the project.

# 2- Preparation of Data Path and Files
The dataset consists of photos in .png format located in folders. Therefore, we cannot read them with pd.read_csv as we do in ML applications. Therefore, it is necessary to organize this data and create a Pandas DataFrame.

# 3- Separating Training, Validation, and Test Data
I separated the training and test data. I also separated some of the training data for validation data.

# 4- Data Loading and Augmentation (Data Enrichment)
In order to use the repeat() function, I created the dataset with tf.data.Dataset. I created a TensorFlow dataset to read image data, preprocess it, and convert its classes into one-hot encoding format, and prepared this dataset appropriately for training, validation, and testing phases, ensuring it was grouped.

# 5- Creating the Model
I created the deep learning model (convolutional neural network) and compiled this model using the categorical_crossentropy loss function with the adam optimization algorithm to perform the image classification task.

# 6- Training the Model
I calculated steps_per_epoch and validation_steps and trained the model with the correct number of data.
The values ​​I got at the end of the 10th epoch are as follows: accuracy: 0.9757 - loss: 0.0738 - val_accuracy: 0.8656 - val_loss: 0.5890

# 7- Performance Analysis and Visuals
I had the Loss and Accuracy graphs drawn in this section so I could more easily observe whether the model was overfit or not.

# 8- Success on the Test Set
I calculated the success on the test set and reached this result. 
Test Accuracy: 0.8564

# 9- Additional Images
In this section, I have included some visuals for the model. The visuals included are:
1- Viewing the First 10 Observations
2- Pixel Density Review
3- Class Distribution Visualization
