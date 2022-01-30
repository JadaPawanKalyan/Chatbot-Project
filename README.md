# Chatbot-Project
The data is spread across three files and contains conversations between two people. So we parse and extract the texts spoken by them.
After extracting we fine-tune a Transformer based T5 model on this dataset, to make the model converse. Just giving the previous text spoken by human does'nt help the model understand the context fully, so we input the past 10 chat sentences as well which makes the model give accurate predictions. 
The model is designed like, At a particular point of prediction time, it takes the previous 10 chat sentences, encode them into a single sentence and generate the reply based on the context.
