In this project, I have completed an end-to-end image classification application. 
I have trained and tested the data using the Multi-class Weather Dataset (MWD):
https://data.mendeley.com/datasets/4drtyfjtfy/1
The MWD contains labelled images representing various weather scenarios. It is a small and popular dataset for practice with image classification.

The project cover the following activities: 
- Data exploration, preparation, and partition:
Generate three CSV files named my_training.csv, my_validation.csv, and my_test.csv that partition the dataset into the training, validation, and test set. Each CSV file contains the following two fields:
• File path
• Image label
The partitions are created randomly, so that the label distribution is similar in each partition   
- Preprocessing and preparation:
Use TensorFlow’s TextLineDataset to generate datasets for training, validation, and test. The datasets need to produce images that are re-sized to dimensions 230 x 230 and 3 channels, and the values of the pixels must be normalised to the range [0, 1].
- Build a simple classifier:
A simple model that contains the following layers:
• A Flatten layer.
• The output layer with the correct size and activation function for this classification task.
Then, train the model with the training data. Use the validation data to determine when to stop training. Finally, test the trained model on the test data and report the accuracy.
- A more complex classifier:
Try a more complex architecture that has 1 or more hidden layers with dropout. For this more complex architecture, use keras-tuner and run it with a reasonable choice of possible parameters: Number of hidden layers, Sizes of hidden layers, Dropout rate and Learning rate.
Perform Error analysis to identify which model generate better accuracy on the test dataset.
- A more complex classifier - Using ConvNets: 
Implement a model that uses a sequence of at least two ConvD, each one followed with MaxPooling2D. Use reasonable numbers for the hyperparameters (number of filters, kernel size, pool size, activation, etc). I do not use pre-trained models for this model.
- Using pre-trained models:
Use MobileNet, pre-trained on imagenet. Add the correct classification layer, and train it with your data. Make sure that MobileNet’s weights is freezed during training.
- Comparative evaluation
Compare all the models to idenitfy which one is the best model.
Test the accuracy of prediction on the best model's test dataset to identify which category is the greatest challenge to predict.

End.


