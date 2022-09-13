# **Pizza Chatbot using Microsoft Azure**
## **Chapter-I**
## Objective

In this project, I would be using QnA Maker Service to make a Chatbot that orders your favourite food like Pizzas, Cakes, Ice Creams and Garlic Bread. It provides rating facility through the given form.
## Problem Statement
Develop a Chatbot for Pizza that greets the customer, provides the menu to choose from the given menu, orders your favorite food from the given digit typed by the customer and provides rating facility through the given form.
## Problem Context
The purpose of chat bots is to support and scale business teams in their relations with customers. It could live in any major chat applications like Facebook Messenger, Slack, Telegram, Text Messages. Chatbot applications streamline interactions between people and services, enhancing customer experience. At the same time, they offer companies new opportunities to improve the customers engagement process and operational efficiency by reducing the typical cost of customer service. This project is focussed on building a custom chatbot that will be your fundamental step of the learning curve of building your own professional chatbots. But you must be tired of the weird chat bots out there in the world which are made for business purposes? In this project, we would be building an extensive Chatbot service, to which you can talk. And talking to a chatbot would not be business driven. It would just be casual conversations. Collaborating with these types of APIs is very much critical as in today's world the popular chatbots do much more than simply having a data-driven conversation; to supplement additional user-oriented features.

## What is a Microsoft Azure QnA Maker Service?
QnA Maker is a cloud-based Natural Language Processing (NLP) service that allows you to create a natural conversational layer over your data. It is used to find the most appropriate answer for any input from your custom knowledge base (KB) of information.
QnA Maker is commonly used to build conversational client applications, which include social media applications, chat bots, and speech-enabled desktop applications.
QnA Maker does not store customer data. All customer data (question answers and chat logs) is stored in the region the customer deploys the dependent service instances in. For more details on dependent services see here.
This documentation contains the following article types:
•	The quickstarts are step-by-step instructions that let you make calls to the service and get results in a short period of time.
•	The how-to guides contain instructions for using the service in more specific or customized ways.
•	The conceptual articles provide in-depth explanations of the service's functionality and features.
•	Tutorials are longer guides that show you how to use the service as a component in broader business solutions.
When to use QnA Maker
•	When you have static information - Use QnA Maker when you have static information in your knowledge base of answers. This knowledge base is custom to your needs, which you've built with documents such as PDFs and URLs.
•	When you want to provide the same answer to a request, question, or command - when different users submit the same question, the same answer is returned.
•	When you want to filter static information based on meta-information - add metadata tags to provide additional filtering options relevant to your client application's users and the information. Common metadata information includes chit-chat, content type or format, content purpose, and content freshness.
•	When you want to manage a bot conversation that includes static information - your knowledge base takes a user's conversational text or command and answers it. If the answer is part of a pre-determined conversation flow, represented in your knowledge base with multi-turn context, the bot can easily provide this flow.



![Picture1](https://user-images.githubusercontent.com/71881295/160241937-dba0468e-ac3b-4ec4-bed0-6f818bf19eed.png)

After you publish your knowledge base, a client application sends a user's question to your endpoint. Your QnA Maker service processes the question and responds with the best answer.
## Problem’s Primary Goals
•	 Setting up a chatbot that can order your requirements (Pizza, Cakes, Ice creams…).

•  Using a QnA Maker Bot service to build Pizza ordering chatbot. 

•  Having a real-world chatbot, to which you can chat like you chatting to a real person and ordering Pizza, Cakes…
## Input
[Spreadsheet.xlsx](https://github.com/sasidhara-kashyap0903/PizzaBot-azure-master/files/8355579/Spreadsheet.xlsx)
## Output
![Picture2](https://user-images.githubusercontent.com/71881295/160243365-5a79dd46-15e2-4473-a12a-858ec57929d1.png)
![Picture3](https://user-images.githubusercontent.com/71881295/160243432-f03bc77b-c102-499c-a3f5-3964b4c580d7.png)
![Picture4](https://user-images.githubusercontent.com/71881295/160243436-fdd6f5dd-5bfb-44e3-8f40-cba95d39d03c.png)
![Picture5](https://user-images.githubusercontent.com/71881295/160243440-558697df-53e7-4ec8-abea-bc840eacb8a1.png)
![Picture6](https://user-images.githubusercontent.com/71881295/160243444-036c8558-276c-4315-aab7-d38f3adc9c34.png)
![Picture7](https://user-images.githubusercontent.com/71881295/160243445-f961f9d4-e100-45a4-9134-2040e026edb5.png)
![Picture8](https://user-images.githubusercontent.com/71881295/160243446-acac3400-42a0-4c69-be81-e5deb98d438e.png)
![Picture9](https://user-images.githubusercontent.com/71881295/160243448-b53a85bb-7691-4f6b-b9aa-9de6e8983cb5.png)
![Picture10](https://user-images.githubusercontent.com/71881295/160243450-b2733e05-78f4-4aa4-b644-d67453434de3.png)
![Picture11](https://user-images.githubusercontent.com/71881295/160243452-4ea2ee56-a57c-4051-a4c1-10aef5cebbc3.png)
![Picture12](https://user-images.githubusercontent.com/71881295/160243453-d1b88f83-369d-4d70-a830-8e0b0c1d0c5c.png)
![Picture13](https://user-images.githubusercontent.com/71881295/160243454-86fb2b8a-e507-4b49-906a-30b71640c6b9.png)
![Picture14](https://user-images.githubusercontent.com/71881295/160243455-3b15a8b3-32fd-49f2-b839-736b012ac792.png)
![Picture15](https://user-images.githubusercontent.com/71881295/160243427-00a7ce9d-984d-4c80-aae0-7ffe7be8c682.png)
![Picture16](https://user-images.githubusercontent.com/71881295/160243430-d07e2e09-36ea-4ddf-8ba1-e28030cabdc3.png)
![Picture17](https://user-images.githubusercontent.com/71881295/160243431-6fa101dd-626e-4dd7-bb49-ca03a874121a.png)
## **Chapter-II**

## Microsoft Azure Bot Framework Architecture
<img width="477" alt="Picture18" src="https://user-images.githubusercontent.com/71881295/160243670-c8026fdc-d60a-426e-92e8-d64178522e22.png">

## Microsoft Azure QnA Maker Development Cycle

![Picture19](https://user-images.githubusercontent.com/71881295/160243758-0622438b-ed0d-4ed0-a9fa-15922a56d8f0.png)
## Life Cycle of a Conversational Bot

![Picture20](https://user-images.githubusercontent.com/71881295/160243891-a71ddc39-a436-444f-9dd1-0fcbed88fc5f.png)

### How to build a bot
Azure Bot Service and the Bot Framework offer an integrated set of tools and services to facilitate the building process. Choose your favorite development environment or command line tools to create your bot. SDKs exist for C#, Java, JavaScript, Typescript, and Python. We provide tools for various stages of bot development to help you design and build bots.
### Plan
As with any type of software, having a thorough understanding of the goals, processes and user needs is important to the process of creating a successful bot. Before writing code, review the bot design guidelines for best practices and identify the needs for your bot. You can create a simple bot or include more sophisticated capabilities such as speech, natural language understanding, and question answering.
### Build
Your bot is a web service that implements a conversational interface and communicates with the Bot Framework Service to send and receive messages and events. Bot Framework Service is one of the components of the Azure Bot Service and Bot Framework. You can create bots in any number of environments and languages.

![Picture34](https://user-images.githubusercontent.com/71881295/160243991-2104e9b0-7dd4-4df7-a65c-7e41ba4913ad.png)
### Test
Bots are complex apps with a lot of various parts working together. Like any other complex app, this can lead to some interesting bugs or cause your bot to behave differently than expected. Before publishing, test your bot. We provide several ways to test bots before they are released for use:
•	Test your bot locally with the emulator. The Bot Framework Emulator is a stand-alone app that not only provides a chat interface but also debugging and interrogation tools to help understand how and why your bot does what it does. The Emulator can be run locally alongside your in-development bot application.
•	Test your bot on the web. Once configured through the Azure portal your bot can also be reached through a web chat interface. The web chat interface is a fantastic way to grant access to your bot to testers and other people who do not have direct access to the bot's running code.

### Publish
When you are ready for your bot to be available on the web, publish your bot to Azure or to your own web service or data center. Having an address on the public internet is the first step to your bot coming to life on your site, or inside chat channels.

### Connect
Connect your bot to channels such as Facebook, Messenger, Kik, Slack, Microsoft Teams, Telegram, text/SMS, and Twilio. Bot Framework does most of the work necessary to send and receive messages from all these different platforms - your bot application receives a unified, normalized stream of messages regardless of the number and type of channels it is connected to. For information on adding channels, see channels topic.

### Evaluate
Use the data collected in Azure portal to identify opportunities to improve the capabilities and performance of your bot. You can get service-level and instrumentation data like traffic, latency, and integrations. Analytics also provides conversation-level reporting on user, message, and channel data.

## Decision Making Between LUIS and QnA Maker

### When to use the QnA Maker?

If your organization has lots of static questions and answers), take advantage of out of the box features of QnA Maker. Upload your static questions and answers into QnA Maker Portal, and your application can call QnA API to search for questions asked by the user on the front-end application and return the response.

### When to use the LUIS?

If you would like to design the application which needs to extract the information from the user’s questions and further process their intents, then use the LUIS.

## Process

<img width="452" alt="Picture21" src="https://user-images.githubusercontent.com/71881295/160244555-43372a2c-a619-4d7a-9acc-b72bdfbab9f2.png">

## Task 1

### Create a Resource Group on Azure

![Picture22](https://user-images.githubusercontent.com/71881295/160244614-76c8fc94-23b6-46f4-acc2-e4f9b308e0bc.png)

## Task2

### Create a QnA Maker Service on Azure

![Picture23](https://user-images.githubusercontent.com/71881295/160244628-2d105988-b0c8-45d0-b375-f5b0454d1d03.png)

## Task3

### Create a Knowledge Base on Azure

![Picture24](https://user-images.githubusercontent.com/71881295/160244659-2b2ca9c3-339d-4b57-9629-710127a2fe02.png)

## Task4

### Create an App Service on Azure

![Picture25](https://user-images.githubusercontent.com/71881295/160244956-c5f1a93c-7e2a-41a7-9a54-cc26b4712cc3.png)

## Task5

### Create a Web App Bot on Azure

![Picture26](https://user-images.githubusercontent.com/71881295/160245269-b89c1643-268f-4010-88c1-a87fd2a44066.png)

## Task6

### Testing my Bot on Azure

![Picture27](https://user-images.githubusercontent.com/71881295/160245121-8c62b017-0cd0-4f19-a8d4-c06aa0ca7922.png)
![Picture28](https://user-images.githubusercontent.com/71881295/160245124-497729e6-c649-4f6a-a8d4-069aa1239f14.png)
![Picture29](https://user-images.githubusercontent.com/71881295/160245125-35d585b0-3301-407d-9cca-9a849fa16561.png)
![Picture30](https://user-images.githubusercontent.com/71881295/160245126-3753df5e-3ffc-4740-9cc4-9319dea9e6ac.png)
![Picture31](https://user-images.githubusercontent.com/71881295/160245115-7f6a40d3-920a-4a05-ab14-8673bc7d9e4f.png)
![Picture32](https://user-images.githubusercontent.com/71881295/160245119-52e497c6-4b00-4702-8dbd-429c7a560fb0.png)
![Picture33](https://user-images.githubusercontent.com/71881295/160245120-d1e5dff3-2b1e-4ba9-9607-939349c54876.png)

## Expected Outcome
By the end of this milestone, you would be having a working chatbot system that orders your favourite food like Pizzas, Cakes, Ice Creams and Garlic Bread to the user along with chatting and provides you rating facility how my service went with you.

## Technologies / Tools Used

• Microsoft Azure QnA Maker Service

• Git Hub

• Microsoft Office

• Microsoft Visual Studio


## URLs
GitHub URL: https://github.com/sasidhara-kashyap0903/PizzaBot-azure-master

Demo URL: https://sites.google.com/view/azurepizzaqnabotcom/home?authuser=0

## Account IDs
Git Hub ID: sasidhara-kashyap0903

Azure Account ID: sasidhara.kashyap@gmail.com

## Acknowledgements
My sincere thanks, to Microsoft for an impressive QnA Maker service on MS Azure Cloud to make the chatbot development easy. It was a wonderful experience learning this and would like to explore more in next two years of my B.Tech. Sincere appreciation to Team of Future Ready Talent who supported and encouraged us to work on this project. 
