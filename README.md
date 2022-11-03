##Objective: -
To build an emotionally aware conversational agent (chatbot) for mental health. 

## Dataset: -

This work makes use of a dataset from Kaggle - [Mental Health FAQ](https://www.kaggle.com/narendrageek/mental-health-faq-for-chatbot). The dataset consists of 98 FAQs about Mental Health. It consists of 3 columns - QuestionID, Questions, Answers. 

## Chatbot Model: -
The repository consists three notebooks for three types of chatbots - Rule-based, Retrieval-based, and Generative-based chatbots. 

1. The rule-based model makes use of TF-IDF along with NLTK's tokenizer for data-preprocessing. The processed data is tested against the expected outcome and cosine similarity is used for evaluation. 
2. For retrieval-based, several Deep Learning models were trained, 
   - Vanilla RNN
   - LSTM
   - Bi - LSTM 
   - GRU 
   - CNN
Retrieval models are trained on JSON file. For all the above models, regularization was used, and based on training and validation accuracies and loss, best model was kept for final comparisons. The CNN model consisted of 3 layers - convolutional neural network (CNN) + an embedding layer + fully connected layer. This model gave the best results. 

3. The generative-based chatbot makes use of Natural Language Processing techniques. It maps user input to an intent, with the aim of classifying the message for an appropriate predefined possible response.
A seq2seq encoder-decoder model that uses LSTMs is implemented for text generation. It predicts a word given in the user input and then each of the next words is predicted using the probability of likelihood of that word to occur. 
  












