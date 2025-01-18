# Gen-AI-using-Llama3.2-LinkedIn-Post_Generator
This tool will analyze posts of a LinkedIn influencer and help them create the new posts based on the writing style in their old posts
![image](https://github.com/user-attachments/assets/80d82ddd-d53f-4248-a87b-f64263b47c4d)

et's say Sunny is a LinkedIn influencer and he needs help in writing his future posts. He can feed his past LinkedIn posts to this tool and it will extract key topics. Then he can select the topic, length, language etc. and use Generate button to create a new post that will match his writing style.

# Technical Architecture
![image](https://github.com/user-attachments/assets/d84276a0-b4ec-43bf-9226-fcebcfece2b7)

Stage 1: Collect LinkedIn posts and extract Topic, Language, Length etc. from it.
Stage 2: Now use topic, language and length to generate a new post. Some of the past posts related to that specific topic, language and length will be used for few shot learning to guide the LLM about the writing style etc.

# Set-up
To get started we first need to get an API_KEY from here: https://console.groq.com/keys. Inside .env update the value of GROQ_API_KEY with the API_KEY you created.
To get started, first install the dependencies using:
 pip install -r requirements.txt
Run the streamlit app:
streamlit run main.py

