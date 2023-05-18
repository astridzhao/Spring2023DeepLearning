# Spring2023 AIT Deep Learning Final Project
Project Title: Enhancing sentiment predictions with ChatGPT-based labeling

Team Members: Astrid Zhao, Avery Chen, Rahul Jain

Project Description: This project aims to train a deep learning model to perform accurate sentiment analysis on any given text. Sentiment analysis is the task of determining the emotion in a given text, classified into categories such as "negative, very negative, neutral, very positive, and positive". We aim to leverage existing datasets: customer movie reviews with sentimental labelings from Stanford Sentiment Treebank to train our model.

In our project, we approach in two ways. 

In both methods, we collect a dataset of labeled sentiments; split the dataset into training, (validation,) and test sets; 

Then, in the first approach, we tokenize the text to convert them into numerical inputs that can be fed into the deep learning model, which includes breaking up the messages into individual words or subwords, and mapping each token to a unique integer. Next, we fine-tune an existing deep learning model, add embedding layers, and create a LSTM (Long-short Term Memory) model to improve performance on the validation set. We believe LSTM is better and more suitable in our project because it allows even more parameters to be learned. In the end, we evaluate the performance of the model on the test set using metrics such as accuracy.

In the second method, we rely on the power fo ChatGPT. We used a newly released technology in ChatGPT: Prompt engineering, which refers to the process of crafting effective and specific instructions or prompts for language models like ChatGPT (such as myself) to elicit desired responses. It involves designing prompts that help guide the model's behavior and produce accurate, relevant, and contextually appropriate outputs. In our case, we give the prompt: “You are a movie review expert and identifying the sentiment of the review. Be as precise, as you can. Identify the sentiment of the input text defined in brackets, and return the sentiment result in brackets too. The return value should be ONLY positive, very positive, neutral, very negative, negative.”  Another cool feature of Prompt engineering is that it gives me not only the sentiment of reviews but also the reasons and evidence why it identifies the sentences as “positive” or “negative”. Also, we provided a list of classic positive, negative, and neutral words to help the chatGPT to enhance the prediction accuracy in the prompt. For example, some of the positive words we gave are 'happy', 'nostalgic', 'Amazing'; negative words are 'negative', 'frustration', 'sad', and etc. However, since the cost of chatGPT, we only feed 100 data to train and test the dataset.

Report Link: https://docs.google.com/document/d/1e98NnQOvsiQ8mSoXA78aiQnGje0bIWacmNBkaYJZV6A/edit?usp=sharing
Slide Link: https://docs.google.com/presentation/d/14oLkuvkPPMOJVig5-y958cpnFKqnuczT9Bc9RbGb8jg/edit?usp=sharing
