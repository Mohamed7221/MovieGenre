# MovieGenre

Movie Genre Prediction Model
This project is a machine learning model designed to predict movie genres based on their plot descriptions using a MultiOutput Naive Bayes classifier. The model uses TF-IDF vectorization to transform text data (movie plots) into numerical features and predicts multiple genres for each movie.

Project Files
train_data.csv: CSV file containing the training data (movie plots and genres).
test_data.csv: CSV file containing the test data (movie plots without genres).
model_evaluation.txt: Text file containing predicted genres for the test data and model evaluation metrics.
Prerequisites
Python 3.x
Required libraries:
pandas
numpy
scikit-learn
tqdm

Dataset Format
Train Data (train_data.csv)
This file contains the following columns:

SerialNumber: A unique identifier for each movie.
MOVIE_NAME: The name of the movie.
GENRE: The genre(s) of the movie (comma-separated if multiple).
MOVIE_PLOT: A brief description or plot of the movie.

Test Data (test_data.csv)
This file contains the following columns:

SerialNumber: A unique identifier for each movie.
MOVIE_NAME: The name of the movie.
MOVIE_PLOT: A brief description or plot of the movie.

How to Run the Model
Prepare your data:

Ensure that the train_data.csv and test_data.csv files are available in the same directory as the code.
Run the code:

The script will automatically load the data from the CSV files, preprocess the text, train the Naive Bayes classifier, and predict the genres for the movies in the test data.
View the results:

The predicted genres will be saved to the file model_evaluation.txt in the format:

Evaluation Metrics
After training, the following metrics will be calculated for the model:

Accuracy: The overall accuracy of the model on the training data.
Precision: The proportion of correctly predicted genres among all predicted genres.
Recall: The proportion of actual genres that were correctly predicted.
F1-Score: The harmonic mean of precision and recall.
