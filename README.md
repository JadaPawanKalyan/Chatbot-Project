# Chatbot-Project
The data is spread across three files and contains conversations between two people. So we parse and extract the texts spoken by them.
After extracting we fine-tune a Transformer based T5 model on this dataset, to make the model converse. Just giving the previous text spoken by human does'nt help the model understand the context fully, so we input the past 10 chat sentences as well which makes the model give accurate predictions. 
The model is designed in such a way like: At a particular point of prediction time, it takes the previous 10 chat sentences, encodes them into a single sentence and generate the reply based on the context.

# Output

User: hello anyone there <br />
Bot: hello there. how are you? <br />
User: i am doing good, thank you <br />
Bot: I'm doing great, thanks. What are you doing?
User: i am presently chatting with you
Bot: That's great. I've been working everywhere since i was.
User: nice. what is your profession right now
Bot: My parents are professors, but i don't have a job
User: that's so sad but i hope you will find a job sooner
Bot: I'm sorry to hear that. What kind of work are you looking for?
User: i am looking for a ml engineer role
Bot: That's cool.

User: Hey
Bot: Hi
User: i like cricket. what about you
Bot: i am not sure what that is
User: cricket is a sport
Bot: i like to watch football.
User: ohh nice. what is your favourite football team
Bot: i like the packers.
User: i dont know about them. can you tell me about packers
Bot: i like to watch them
User: do you know about india?
Bot: i don't know about it
User: india is a huge country
