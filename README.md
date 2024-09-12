# WhatsappGPT
A chat GPT-powered Whatsapp bot
I am pretty lazy about opening the ChatGPT website, logging in, and then accessing the website. So I could make a bot that could be accessed easily. My seniors have talked a lot about OpenAI API, so I decided to make myself my bot And implement it on one of my most used apps, WhatsApp.
This is the code.

**Limitations:**
1. This bot only works when you are locally hosting it. Case you want to host it 24*7, you need to upload it to a web server like AWS, which I don't feel comfortable putting my debit card details
2. as there is only limited time access to these APIs so, in the end, you may need to pay to use them forever
3. you need to install a lot of stuff. Trust me
4. there is a type error. I don't know why it is coming even when I am returning a string
   
**Procedure to use it:**
1. use pip to install Twilio, requests, python-ngrok, request, python-dotenv, openAI
2. create an account at Twilio and activate the send by WhatsApp message. Get the WhatsApp number, your authorization side, and the token and change it in the .env file and the form variable WhatsApp: the number they provide
3.  Create an account in openAI, create an API key, and put it in the env file
4.  now create a folder openai_caht and insert the e.nv file and wa_bot file
5.  now open the terminal, type ngrok http 5020(the port number can be any port number in the run file),  and run the command. It will install the ngrok if not installed
6.  now, it will give one receiving link. Take that link, put it in the sandbox WhatsApp setting under the receiving link, and add '\message' at the end of the app to connect to the Flask app we will be running
7.  now run the run python file, and you can access ChatGPT in WhatsApp

**Further improvement:**
1. we can use sms api to implement simple text messages, and that will be beneficial for many people who live in remote places and will have access to the power of chatGPT
2. we can just implement other AI like DALL-e
3. we can host it 24*7 on a cloud. I will do so once I come across free cloud services
   
