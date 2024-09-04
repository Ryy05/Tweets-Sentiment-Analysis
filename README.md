# Sentiment Analysis Using Bidirectional LSTM

**Project Overview**

This project demonstrates the application of a Bidirectional Long Short-Term Memory (BiLSTM) model for sentiment analysis on a dataset of tweets. The objective is to classify tweets into positive or negative sentiment based on their textual content.

**Dataset**

The dataset used is a subset of the Sentiment140 dataset, which consists of 1.6 million tweets labeled as positive or negative. For faster processing, a smaller subset was used.

**Model Architecture**

The model is built using TensorFlow and Keras and includes the following layers:

**Embedding Layer:** 
Converts words into dense vectors of fixed size.
**Bidirectional LSTM Layers:** T
wo layers with 64 and 32 units respectively, to capture context from both directions.
**Dropout Layers:** 
Used for regularization to prevent overfitting.
**Dense Layer:** 
Final layer with a sigmoid activation function for binary classification.

**Data Preprocessing**

The data preprocessing steps include:

Cleaning the Tweets: Removing URLs, special characters, and unnecessary spaces.
Tokenization: Converting text into sequences of integers.
Padding: Ensuring all sequences have the same length by padding shorter sequences with zeros.
Training the Model
The model is trained for 5 epochs using the Adam optimizer and binary cross-entropy loss function. The training process is monitored with accuracy as the primary metric.

**Evaluation**

The model is evaluated on a test set, and its performance is measured using accuracy, confusion matrix, and classification report.

**Visualizations**

Various visualizations are included to better understand the data and model performance:

**Word Clouds:** 
Visual representation of the most frequent words in positive and negative tweets.
Accuracy and Loss Plots: Visualizations of the training and validation accuracy and loss over epochs.
Installation

**To run this project locally:**

Clone the repository: git clone <repository-link>
Install the required dependencies: pip install -r requirements.txt
Usage
Once the environment is set up, you can train the model and evaluate it by running the provided Python scripts.

**Results**

The final model achieved an accuracy of approximately [insert accuracy]% on the test set. The confusion matrix and classification report provide further insights into the model's performance.

**Conclusion**

This project successfully demonstrates the effectiveness of BiLSTM for sentiment analysis. The model is able to classify sentiments in tweets with reasonable accuracy.


**Potential improvements could include:**

Using a more complex model or pre-trained transformers like BERT.
Expanding the dataset to improve model generalization.
Fine-tuning hyperparameters for better performance.
