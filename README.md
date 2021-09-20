# Chatbot

## A simple chatbot that utilizes deep learning techniques to initiate a conversation. 
#### ** Since this is a simple chatbot model, we will stick to the purposes of an FAQ style intent sheet. The intent file can be modified as required, and the program will function the same.

### Libraries used - 
* #### Numpy
* #### NLTK
* #### TensorFlow
* #### TFLearn

### Step-by-Step Process - 
* #### Intents File - This can be created by simply opening a JSON file and using a set format. This will be acting as our training data. Whenever we talk to the chatbot, the answers it gives us will be based on its training with this intents file. Therefore, the more nuanced the file, the better the final conversation. For the purposes of this particular chatbot, I have kept the intents file relatively simple, opting to base it on an actual file I found online. 
![image](https://user-images.githubusercontent.com/43636138/133967400-464ea99a-1ef7-4528-9b1e-67060aaeaa3c.png)
* #### Data Extraction - The intents file that has been loaded has to be understood by the program, and therefore I will be extracting the data. The string values will be converted to token values by using *nltk tokenizer*. This will also generate a tag for each token. Each of the unique words in the file will be stored as part of a pattern. The patterns will go in a separate list, and the tags will go in a separate list.
![image](https://user-images.githubusercontent.com/43636138/133967616-168b3c96-ed00-4b0d-8e19-1c93aa8a0806.png)
* #### Stemming - There are more than a million words in the English vocabulary. Assuming that the computer is/will be well versed with them is futile. Stemming helps reduce the cumbersome task of building vocabulary by presenting a more generalised meaning to root words and extensions, creating a far more nuanced sense of the vocabulary by putting in little effort.
![image](https://user-images.githubusercontent.com/43636138/133967839-a67a1144-baf4-48c4-b5a9-0731ed5fb1c4.png)
* #### Bag of Words - Strings will not be efficient for a computer to process to gain accurate prediction results. Thus, I converted the strings to numerical values. I will assign the value of 1 to words that are present in the list of words from the model's vocabulary, and 0 for the words that are absent. I will also create an output list that replicates this process to a numpy training array.
![image](https://user-images.githubusercontent.com/43636138/133967908-e73d781f-9b2e-457e-aef0-5a551f4d6f9e.png)
* #### Model - The processed data has to now be passed through a model for training. The model in question is a two layer simple neural network. This model's accuracy can be changed by playing around with the numbers, and can be saved for later use.
![image](https://user-images.githubusercontent.com/43636138/133967967-0f5881dc-eb6a-46ba-87e4-9c4e65e9db76.png)
* #### Predictions - After the model has been trained and invoked, a user can type a sentence of choice. If the JSON file is nuanced enough, it can take in more conversations, queries and get better acquainted with the process. At the same time, in the event that it does not understand the conversation, I have added a failsafe. 
![image](https://user-images.githubusercontent.com/43636138/133968019-00978775-b96e-4973-925b-5446bbe00775.png)

#### Find me here - 
* #### [Github](https://github.com/deadven7) 
* #### [Kaggle](https://www.kaggle.com/amaanvora) 
* #### [LinkedIn](https://www.linkedin.com/in/amaan-vora/) 
