# WhatsappGPT
A chat GPT-powered Whatsapp bot
I am pretty lazy to open the ChatGPT website, log in then access the website. So I could make a bot that could be accessed easily. My seniors have talked a lot about OpenAI API, so I decided to make myself my bot And implement it on one of my most used apps Whatsapp.
This is the code.
**Limitations:**
1. This bot only works when you are locally hosting it. Case you want to host it 24*7, you need to upload it to a web server like AWS, which I don't feel comfortable putting my debit card details
2. as there is only limited time access to these APIs so, in the end, you may need to pay to use them forever
3. you need to install a lot of stuff. Trust me
4. there is a type error. I don't know why it is coming even when I am returning a string
**Procedure to use it:**
1. use pip to install Twilio, requests, python-ngrok, request, python-dotenv,openai
2. create an account at Twilio and activate the send by WhatsApp message. Get the whatsapp number, your authorization sid and the token and change it in .env file and the from variable WhatsApp: the number they provide
3.  Create an account in open ai and create api key and put it in env file
4.  now create a folder openai_caht inser the e.nv file and wa_bot file
5.  now open terminal type ngrok http 5020(port number can be any port number in run file)  and run the command it will install the ngrok if not installed
6.  now it will give one reveiving link take that link and put it in sandbox whatsapp setting under receiving link and add '\message' in end of the app to connect to the flask app we will be running
7.  now run the run python file and you can acess chatgpt in whatsapp
**Further improvement:**
1. we can use sms api to implement simple text messages and that will be beneficial for many people who live in remote places and will have access to power of chatGPT
2. we can just iplment other Ai like DALL-e
3. we can host it 24*7 on cloud I will do so once I came across free cloud services
   
