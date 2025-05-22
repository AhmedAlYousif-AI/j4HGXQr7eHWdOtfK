# MonReader 

Introduction:
Developing an intelligent document scanning system for Hardware and vision field that could help blinders, and researchers for an automatic scanning of the content based on flipping the pages of the book.


Data Description:
The Dataset is consists of 2998 images, divided into training (2392 images) and testing ( 597 images) folders. Each folder contains two files (flip) and (notflip) for categorizing the images. 


Methodology:
1. Importing the images into specified paths for each set of the dataset. data path for importing the entire dataset, training_path for importing the training set, and testing_path for importing the testing set.
2. Resizing all images of the imported dataset into 224 x 224 shape.
3. Labeling the dataset as same as its structure for 'flip' and 'notflip' images.
4. Assigning the dataset training set and testing set paths into training_data directory and testing_data directory, this process is essential for passing the dataset into the Neural Network while building the model.
5. Building the model using Convolutional Neural Network (CNN), while setting 4 Convolutional layers including and starting from the Input layer while using 'relu' activation function, 1 Flatten layer, and 1 Fully-Connected Dense layer with 'relu' activation function, reaching to the Output layer while using 'sigmoid' activation function.
6. Training the model while initialzing the batch_size = 150, epochs=60, verbose=2, and adding Early Stopping technique to avoid over-training and wasting the resources for the hardware when the training is not improving.
7. Plotting the Training result using Matplotlib library Python.
8. Evaluating the result of the model using Testing dataset.
9. Saving the model.


Conclusion:
By applying Convolutional Neural Networks (CNNs), the result reached to above 100% of Accuracy for detecting the images using training dataset, and 99.92% of Accuracy using testing dataset.
