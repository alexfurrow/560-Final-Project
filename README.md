# DSO 560 Final Project
<font size="3"> Part 1: Product Attribution for Women's Fashion Items</font>

- Authored by Team Yellow: Alex Furrow, Sandra Chen, Bo Kyung Cho, Kathy Chen, Rachel Sung
- As prompted by Professor Yu Chen
- In collaboration with ThreadTogether

Categories and Tags Chosen for Attribute Prediction:
- Style: 'classic', 'modern', 'casual', 'romantic', 'glam', 'businesscasual', 'edgy', 'retro', 'androgynous', 'boho', 'athleisure',
- Embellishments: 'studs', 'embroidery', 'trim', 'ruffles', 'mesh', 'fringe', 'lace', 'buckles', 'sequins', 
- Occasion: 'daytonight', 'nightout', 'work', 'weekend', 'vacation', 'workout', 'coldweather', 
- Category: 'top', 'onepiece', 'bottom', 'shoe', 'sweater', 'accessory', 'blazerscoatsjackets','sweatshirthoodie'
- Dry Clean Only: 'yes', 'no'

 Files in this Repo:
 1) Classification model(doc2vec).ipynb - an attempt at using a logistic regression on doc2vec embeddings that had 83.1% accuracy on the validation data set
 2) Data-Preprocessing-Sandra-Chen.ipynb - data preprocessing steps, including regex cleaning, stopword removal, lemmatization, etc
 3) Initial Look at the Data.ipynb - this file is to document the initial data exploration 
 4) One Hot Encoding and Duplicate Removal.ipynb - for all attributed data (training data) each of the tags are one hot encoded and duplicates on the product_id are removed, this is for training models. The result of this file is the "Encoded Data" folder
 5) Encoded data - this folder contains all the one hot encodings for each of the tags. These files are required to run the "Standard NN.ipynb" model, the model in the "Deep Learning Prediction" folder, and the models in the "RNN Models" folder, and the "Classification model(doc2vec).ipynb
 6) Deep Learning Prediction - this folder contains a model that trains on the full set of training data and outputs labels for the test data set (i.e. non-attributed data). It includes the resulting output.csv. This, however, is not the group's submission, it is the backup.
 7) RNN Models - this folder contains recurrent neural network models using glove embedding had a prediction accuracy of 85.3%
 8) Standard NN.ipynb - this model attempts classification using a deep learning neural network with Keras Embedding() and had an accuracy of 84.2% 
 
Goals:
1) Extract retail clothing information (data gathered from retail websites) and preprocess it for modeling
2) Try different models with different embeddings to predict select attribtes on untagged data 
3) Predict attributes using the best model/embedding combo


<font size="4"><u> Outline of Steps Taken </u> </font>

    1) Preprocessing Data
        - Columns selected: name, description, brand category 
        - Cleaning, removing stopwords lemmatization
        - One hot encoding & de-duplication
    2) Word Embedding and Model Building
        - Glove embedding
        - TFIDF
        - Doc2vec
        - Embedding() from Keras
    3) Model Building
        - Recurrent Neural Network (RNN)
        - Logistic Regression
        - Deep Learning Neural Network
        - Logistic & Decision Tree Combination
    4) Model Accuracy
        - Recurrent Neural Network (RNN): 85.3%
        - Logistic Regression: 83.1%
        - Deep Learning Neural Network: 84.2%
        - Logistic & Decision Tree Combination: 86.8%
    5) Model Selection
        - Models compared by test accuracy (Logistic & Decision Tree Combination)
    6) Prediction
        - Excel Output Provided
    7) Demo/Test Function for Project Evaluation



 
