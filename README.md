A project where I worked on introductory level classification, data analysis, model development and evaluation techniques in the fields of deep learning and artificial neural networks (ANN) with a large scale fish dataset.

Dataset: https://www.kaggle.com/datasets/crowww/a-large-scale-fish-dataset

# Project Stages
===

# 1- Required Libraries
First of all, I imported the necessary libraries in the project.

# 2- Preparation of Data Path and Files
The dataset consists of photos in .png format located in folders. Therefore, we cannot read them with pd.read_csv as we do in ML applications. Therefore, it is necessary to organize this data and create a Pandas DataFrame.

# 3- Separating Training, Validation, and Test Data
I separated the training and test data. I also separated some of the training data for validation data.

# 4- Data Loading and Augmentation (Data Enrichment)
In order to use the repeat() function, I created the dataset with tf.data.Dataset. I created a TensorFlow dataset to read image data, preprocess it, and convert its classes into one-hot encoding format, and prepared this dataset appropriately for training, validation, and testing phases, ensuring it was grouped.

# 5- Creating the Model
I created a neural network model (Artificial Neural Network - ANN) using TensorFlow's Keras API, which consists of several layers including input, flattening, fully connected layers, dropout layers for regularization, and an output layer with softmax activation for classification, and then compiled it with an Adam optimizer and categorical crossentropy loss, incorporating early stopping to prevent overfitting

# 6- Training the Model
In this code, the steps_per_epoch and validation_steps are calculated based on the lengths of the training and validation datasets divided by the batch size, and then the model is trained using the fit method for 20 epochs with early stopping to prevent overfitting, while handling any potential errors that may occur during the training process.

# 7- Loss and Accuracy Graphs
I had the Loss and Accuracy graphs drawn in this section so I could more easily observe whether the model was overfit or not.

# 8- Success on the Test Set
I calculated the success on the test set and reached this result. 

# 9- Additional Images
In this section, I have included some visuals for the model. The visuals included are:
1- Viewing the First 10 Observations
2- Pixel Density Review
3- Class Distribution Visualization
