Developer boilerplate to build chat bots using NLP services.

**************************Integarting with Dialogflow NLP services************************************

Google dialogflow setup and configuration

1. Please login dialogflow using below-mentioned link and on successful login navigate to the console

	 https://dialogflow.com


2. Create a new agent to start with NLP service

3. Copy client key after successful creation of agent for further usage



Dialogflow training

1. create new intent to add utterances

2. save the intents after adding utterances and it will automatically train the agent


Connectivity with bot connect

1. git clone https://github.com/divergence-labs/Bot-Connect.git 

2. create .env file and place your dialogflow client key which you copied earlier

3. npm install

4. npm start

Microservices details

1. API details to interact with Dialogflow NLP service

POST method

API endpoint : http://localhost:3000/user/expressions/dialogflow

Body request:
{
	"user_expressions":"EXPRESSIONS"
}

**************************Integarting with LUIS NLP services************************************
Microsoft LUIS setup and configuration

1. Please login to LUIS using below-mentioned link and on successful login navigate to the console

	 https://luis.ai/home 


2. Create a new application to start with NLP service

3. Copy endpoints,primary key and App ID after successful creation of application



LUIS training

1. create new intent to add utterances

2. save the intents after adding utterances and train the agent


Connectivity with bot connect

1. git clone https://github.com/divergence-labs/Bot-Connect.git 

2. create .env file and place your LUIS endpointURL,primary key and appID which you copied earlier

3. npm install

4. npm start

Microservices details

1. API details to interact with LUIS  NLP service

POST method

API endpoint : http://localhost:3000/utterances/luis

Body request:
{
	"utterances":"EXPRESSIONS"
}
 