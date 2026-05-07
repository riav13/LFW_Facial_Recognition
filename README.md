LFW (Labelled Faces in the Wild) Facial Recognition Machine Learning Project


Dataset: The dataset used was Kaggle's LFW dataset which is a widely used dataset used for understanding facial recognition algorithms in machine learning. It contains a total of 
13,233 images of 5,749 people. For this project, I used 5 people for training and testing, each with 42-530 sample images of the person. 
https://www.kaggle.com/datasets/jessicali9530/lfw-dataset

Goal/Objective: The goal was to explore PCA (Principal Components Analysis) and Random Forest(RF) to see if dimensionality reduction helps with classification of people.
Principal Components Analysis reduces the feature space into a specified amount of components which are supposedly the most important features for distinguishing between people. 
PCA also requires less computational cost compared to a method that uses the whole feature space with Random Forest, so I wanted to test out this tradeoff to see if it is also able to 
classify just as well/semi-accurately. 

Steps:
1.Selecting People and Converting Images to Vectors
2.Looking at the data (eigenfaces) and showing the images transformed
3.Splitting into train and test sets (75-25 split)
4.Applying PCA to get features with maximum variance (the components represent the features that PCA thinks are important when distinguishing between faces)
  -visualize PCA components as eigenfaces to see which components 
5.Training Random Forest Classifier Using the Components from PCA
6.Testing Accuracy (Train-Test Accuracy, Confusion Matrix)
