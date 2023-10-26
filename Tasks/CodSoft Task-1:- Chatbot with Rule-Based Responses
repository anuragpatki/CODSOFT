import re

# Define a dictionary of rules
rules = {
    "(hi|hello|hey)": "Hello! How can I help you today?",
    "(what is your name|who are you)": "My name is Jarvis. I am a large language model.",
    "(what is the time)": "The time is currently 17:14 PST on 2023-10-26.",
    "(how are you doing)": "I am doing well, thank you for asking!",
    "(goodbye|bye)": "Goodbye! Have a nice day!",
     "(good morning)": "Good morning! How can I help you today?",
    "(good afternoon)": "Good afternoon! How can I help you today?",
    "(good evening)": "Good evening! How can I help you today?",
    "(have a good day)": "You too! Have a great day!",
    "(see you later)": "See you later! Have a great day!",
    "(how are you)": "I am doing well, thank you for asking!",
    "(what is the weather like today)": "The weather in Satara, India is currently 27 degrees Celsius and sunny.",
    "(what is the news today)": "Here is a summary of the top news stories today...",
    "(what are your features)": "I can generate text, translate languages, write different kinds of creative content, and answer your questions in an informative way.",
    "(how much do you cost)": "I am currently free to use.",
    "(how do I use you)": "To use me, simply type a question or request and I will do my best to respond.",
    "(i would like to book an appointment with dr. smith)": "Sure. What date and time would you like to book your appointment for?",
    "(i would like to order a size 10 blue t-shirt)": "Sure. What is your shipping address?",
    "(i am having trouble with my account)": "I can help you with that. Please describe the problem in more detail."

}

# Define a function to match user queries to rules
def match_rule(query):
    for pattern, response in rules.items():
        if re.match(pattern, query):
            return response
    return None

# Define a function to generate a response to a user query
def generate_response(query):
    response = match_rule(query)
    if response is None:
        response = "I don't understand your query. Please try again."
    return response

# Start the chatbot loop
while True:
    user_query = input("User: ")
    response = generate_response(user_query)
    print(f"Chatbot: {response}")
