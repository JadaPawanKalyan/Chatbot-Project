# Chatbot-Project
The data is spread across three files and contains conversations between two people. So we parse and extract the texts spoken by them.
After extracting we fine-tune a Transformer based T5 model on this dataset, to make the model converse. Just giving the previous text spoken by human does'nt help the model understand the context fully, so we input the past 10 chat sentences as well which makes the model give accurate predictions. 
The model is designed in such a way like: At a particular point of prediction time, it takes the previous 10 chat sentences, encodes them into a single sentence and generate the reply based on the context.

# Output

User: hello anyone there <br />
Bot: hello there. how are you? <br />
User: i am doing good, thank you <br />
Bot: I'm doing great, thanks. What are you doing? <br />
User: i am presently chatting with you <br />
Bot: That's great. I've been working everywhere since i was. <br />
User: nice. what is your profession right now <br />
Bot: My parents are professors, but i don't have a job <br />
User: that's so sad but i hope you will find a job sooner <br />
Bot: I'm sorry to hear that. What kind of work are you looking for? <br />
User: i am looking for a ml engineer role <br />
Bot: That's cool. <br />
<br />
<br />
User: Hey <br />
Bot: Hi <br />
User: i like cricket. what about you <br />
Bot: i am not sure what that is <br />
User: cricket is a sport <br />
Bot: i like to watch football. <br />
User: ohh nice. what is your favourite football team <br />
Bot: i like the packers. <br />
User: i dont know about them. can you tell me about packers <br />
Bot: i like to watch them <br />
User: do you know about india? <br />
Bot: i don't know about it <br />
User: india is a huge country <br />
