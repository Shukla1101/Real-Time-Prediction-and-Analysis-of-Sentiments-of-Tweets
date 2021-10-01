# Real-Time-Prediction-and-Analysis-of-Sentiments-of-Tweets
Real time, Time-based analysis of sentiments of tweets about specific topics from a given location.

Data Preprocessing- Data is preprocessed for semantic analysis before creating the RNN model and
LSTM architecture. 
For the preprocessing of data, Load the dataset obtained into the system and visualize it using python libraries like matplotlib,pandas etc (identifying the
important parameters which are dependent variables in the dataset). 
Next we convert all the reviews into lowercase to make them similar in pattern.  After this, Data Cleaning is necessary for efficient working of the model, For
Data Cleaning, Remove all the punctuation from the reviews as they are not relevant while predicting the sentiments, Remove all the un-useful waste data
before actual work start . 
At last,Create a list of reviews using python library (pandas) as dependent
variables. 

Tokenization- 
 Tokenization is performed before sentiment analysis for classification of thedata over different sentiments.  For this,Create a vocabulary to integer mapping dictionary to tokenize each words. 
 Encode the words so that the model can easily recognize it as a variable or a parameter. 
 Analyze the length of the reviews. 
 Now to make the dataset efficient we need to remove the outliners present in it. So we find all the reviews which are extremely long or extremely short and remove them to maintain consistency in the dataset.
 Now the main task is to pad/truncate the reviews in remaining data.

Sentiment Analysis-
 We perform Sentiment Analysis by our tokenized bag of words using python libraries (NLTK / TEXTBLOB) to process the textual data. 
 Sentiment Analysis is performed for classification of data over the different sentiments before analyzing it on the time series. 
 We create a sparse matrix of the words for sentiment Analysis. 
 After this we need to apply time series on the reviews which are now in the form of sparse matrix as a model of bag of words.

Splitting- 
 Next we split the dataset into 3 parts:
1. Training set
2. Validation set
3. Testing set
 With the help of K-Fold validation we split the dataset into training and testing set using various combinations to make our prediction model more efficient
and robust. 
 The data is then divided into various batches as we are applying batch processing in our model.

Implementing RNN with LSTM Architecture- 
 After this we create a classifier of recurrent neural network using deep learning techniques for creating time series of the data obtained from sentiment analysis
and we then apply the LSTM architecture over it to remove the problem of long distance dependencies ,exploding gradient and vanishing gradient.
 Now we create a neural network of multiple layers (number of layers will be determined during testing period of project for performance evaluation). Then
the model is trained for suitable number of epochs. 

Training and Testing- 
 Finally the model created is tested for the test data as well as for the user generated data and evaluated for the efficiency
