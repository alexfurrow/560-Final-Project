# DSO 560 Final Project
<font size="3"> Part 1: Product Attribution for Women's Fashion Items</font>


- Authored by Team Yellow: Alex Furrow, Sandra Chen, Bo Kyung Cho, Kathy Chen, Rachel Sung
- As prompted by Professor Yu Chen
- In collaboration with ThreadTogether

Goals:
1) Attribute Data: extract retail clothing information (data gathered from retail websites)
2) Attribution Tool: create app that parses text and is repeatable given new data (any new data would need to be organized to be input: descriptions, tags, other metadata

<font size="4"><u> Outline </u> </font>

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
        - Logistic & Decision Tree Combination: ??
    
    5) Model Selection
        - Models compared by test accuracy
    6) Prediction
        - Excel Output Provided
        
 
