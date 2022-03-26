# PizzaBot-azure-master
Developing a Chatbot using Azure QnA Maker service and developed this for a pizza restaurant which greets and communicates with customer and provide them the menu and takes the order. When the customer checks about the parcel service it says that the facility is coming soon.
Project Work on

***“Pizza Chatbot Development”***

Using

***Azure QnA Maker Service***

***Chapter -I***

![](media/image1.png){width="2.3in" height="0.5in"}

Submitted by

***Sasidhara Kashyap Chaturvedula***

**Second year B. Tech, GRIET, Hyderabad**

Submitted to

***Future Ready Talent***

![](media/image2.png){width="1.5083333333333333in"
height="0.7166666666666667in"}**\
**

**Objective**
=============

In this project, I would be using ***QnA Maker Service*** to make a
***Chatbot*** that orders your favourite food like Pizzas, Cakes, Ice
Creams and Garlic Bread. It provides rating facility through the given
form.

**Problem Statement**
=====================

Develop a ***Chatbot*** for ***Pizza*** that greets the customer,
provides the menu to choose from the given menu, orders your favorite
food from the given digit typed by the customer and provides rating
facility through the given form.

**Problem Context**
===================

The purpose of chat bots is to support and scale business teams in their
relations with customers. It could live in any major chat applications
like Facebook Messenger, Slack, Telegram, Text Messages. Chatbot
applications streamline interactions between people and services,
enhancing customer experience. At the same time, they offer companies
new opportunities to improve the customers engagement process and
operational efficiency by reducing the typical cost of customer service.
This project is focussed on building a custom chatbot that will be your
fundamental step of the learning curve of building your own professional
chatbots. But you must be tired of the weird chat bots out there in the
world which are made for business purposes? In this project, we would be
building an extensive Chatbot service, to which you can talk. And
talking to a chatbot would not be business driven. It would just be
casual conversations. Collaborating with these types of APIs is very
much critical as in today's world the popular chatbots do much more than
simply having a data-driven conversation; to supplement additional
user-oriented features.

**What is a Microsoft Azure QnA Maker Service?**
================================================

QnA Maker is a cloud-based Natural Language Processing (NLP) service that allows you to create a natural conversational layer over your data. It is used to find the most appropriate answer for any input from your custom knowledge base (KB) of information.
===============================================================================================================================================================================================================================================================

QnA Maker is commonly used to build conversational client applications,
which include social media applications, chat bots, and speech-enabled
desktop applications.

QnA Maker does not store customer data. All customer data (question
answers and chat logs) is stored in the region the customer deploys the
dependent service instances in. For more details on dependent services
see [here](https://docs.microsoft.com/en-us/azure/cognitive-services/qnamaker/concepts/plan?tabs=v1).

This documentation contains the following article types:

-   The [quickstarts](https://docs.microsoft.com/en-us/azure/cognitive-services/qnamaker/quickstarts/create-publish-knowledge-base) are
    > step-by-step instructions that let you make calls to the service
    > and get results in a short period of time.

-   The [how-to
    > guides](https://docs.microsoft.com/en-us/azure/cognitive-services/qnamaker/how-to/set-up-qnamaker-service-azure) contain
    > instructions for using the service in more specific or
    > customized ways.

-   The [conceptual
    > articles](https://docs.microsoft.com/en-us/azure/cognitive-services/qnamaker/concepts/plan) provide
    > in-depth explanations of the service's functionality and features.

-   [**Tutorials**](https://docs.microsoft.com/en-us/azure/cognitive-services/qnamaker/tutorials/create-faq-bot-with-azure-bot-service) are
    > longer guides that show you how to use the service as a component
    > in broader business solutions.

When to use QnA Maker
---------------------

-   **When you have static information** - Use QnA Maker when you have
    > static information in your knowledge base of answers. This
    > knowledge base is custom to your needs, which you've built with
    > documents such as [PDFs and
    > URLs](https://docs.microsoft.com/en-us/azure/cognitive-services/qnamaker/concepts/data-sources-and-content).

-   **When you want to provide the same answer to a request, question,
    > or command** - when different users submit the same question, the
    > same answer is returned.

-   **When you want to filter static information based on
    > meta-information** -
    > add [metadata](https://docs.microsoft.com/en-us/azure/cognitive-services/qnamaker/how-to/metadata-generateanswer-usage) tags
    > to provide additional filtering options relevant to your client
    > application's users and the information. Common metadata
    > information
    > includes [chit-chat](https://docs.microsoft.com/en-us/azure/cognitive-services/qnamaker/how-to/chit-chat-knowledge-base),
    > content type or format, content purpose, and content freshness.

-   **When you want to manage a bot conversation that includes static
    > information** - your knowledge base takes a user's conversational
    > text or command and answers it. If the answer is part of a
    > pre-determined conversation flow, represented in your knowledge
    > base with [multi-turn
    > context](https://docs.microsoft.com/en-us/azure/cognitive-services/qnamaker/how-to/multi-turn),
    > the bot can easily provide this flow.

**What is a Knowledge Base?**
=============================

QnA Maker [imports your content](https://docs.microsoft.com/en-us/azure/cognitive-services/qnamaker/concepts/plan) into a knowledge base of question-and-answer pairs. The import process extracts information about the relationship between the parts of your structured and semi-structured content to imply relationships between the question-and-answer pairs. You can edit these question-and-answer pairs or add new pairs.
===================================================================================================================================================================================================================================================================================================================================================================================================================================

The content of the question-and-answer pair includes:

-   All the alternate forms of the question

-   Metadata tags used to filter answer choices during the search

-   Follow-up prompts to continue the search refinement

![](media/image3.png){width="6.268055555555556in" height="1.80625in"}

After you publish your knowledge base, a client application sends a
user's question to your endpoint. Your QnA Maker service processes the
question and responds with the best answer.

**Problem’s Primary Goals **
============================

-   Setting up a chatbot that can order your requirements (Pizza, Cakes,
    Ice creams…).

-   Using a QnA Maker Bot service to build ***Pizza*** ordering chatbot.

-   Having a real-world chatbot, to which you can chat like you chatting
    to a real person and ordering Pizza, Cakes…

**Input**
=========

  ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  S/NO   Intent Name       Training Phrase    Response Phrase
  ------ ----------------- ------------------ ----------------------------------------------------------------------------------------------------------------------------------------------------
  1      greetings         hello pizza bot    **Hello, how can I help you?**
                                              
                                              **This is Kashyap at your service.**

  2      showMenu          show me the menu   ***Menu (Please TYPE 1 to 9 to access the items and TYPE 10 to Quit)***
                                              
                                              **I. Pizza Cost**
                                              
                                              **1. Pineapple Pizza 20\$**
                                              
                                              **2. Corn Pizza 50\$**
                                              
                                              **3. Paneer Pizza 75\$**
                                              
                                              **4. Non-Veg Pizza 100\$**
                                              
                                              **II. Cakes**
                                              
                                              **5. Chocolate Cake 50\$**
                                              
                                              **6. Strawberry Cake 50\$**
                                              
                                              **III. Ice Creams**
                                              
                                              **7. Vanilla Ice Cream 50\$**
                                              
                                              **8. Butter Scotch Ice Cream 50\$**
                                              
                                              **IV. Garlic Bread**
                                              
                                              **9. Garlic Bread 75\$**
                                              
                                              **V.Quit**
                                              
                                              **10. Quit**
                                              
                                              ***(You have to assume that you have already paid to those items shown above)***

  3      order             1                  **You have ordered Pineapple Pizza, do you want to continue?**
                                              
                                              **please TYPE (confirm or no)**

                           2                  **You have ordered Corn Pizza, do you want to continue?**
                                              
                                              **please TYPE (confirm or no)**

                           3                  **You have ordered Paneer Pizza, do you want to continue?**
                                              
                                              **please TYPE (confirm or no)**

                           4                  **You have ordered Non-Veg Pizza, do you want to continue?**
                                              
                                              **please TYPE (confirm or no)**

                           5                  **You have ordered Chocolate Cake, do you want to continue?**
                                              
                                              **please TYPE (confirm or no)**

                           6                  **You have ordered Strawberry Cake, do you want to continue?**
                                              
                                              **please TYPE (confirm or no)**

                           7                  **You have ordered Vanilla Ice Cream, do you want to continue?**
                                              
                                              **please TYPE (confirm or no)**

                           8                  **You have ordered Butterscotch Ice Cream, do you want to continue?**
                                              
                                              **please TYPE (confirm or no)**

                           9                  **You have ordered Garlic Bread, do you want to continue?**
                                              
                                              **please TYPE (confirm or no)**

                           10                 **Thank You for visiting our restaurant please give us a rating on this form: [Azure Pizza Chatbot Service](https://forms.gle/KQQ3FLruEKUPnw8m7)**

  4      orderConfirm      confirm            **You have confirmed your order, it is being ready and you will get your order within 45 mins. Thank You.**

  5      orderNotConfirm   no                 **Please choose any other item from the Menu or TYPE 10 to quit.**
  ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Output**
==========

![](media/image4.png){width="6.268055555555556in"
height="1.8722222222222222in"}

![](media/image5.png){width="6.572916666666667in"
height="2.8020833333333335in"}

![](media/image6.png){width="6.268055555555556in" height="2.7715277777777776in"}
================================================================================

![](media/image7.png){width="6.268055555555556in"
height="2.8979166666666667in"}

![](media/image8.png){width="6.268055555555556in"
height="2.8048611111111112in"}

![](media/image9.png){width="6.268055555555556in"
height="2.785416666666667in"}

![](media/image10.png){width="6.268055555555556in"
height="2.776388888888889in"}

![](media/image11.png){width="6.268055555555556in"
height="2.763888888888889in"}

![](media/image12.png){width="6.268055555555556in"
height="2.7416666666666667in"}

![](media/image13.png){width="6.268055555555556in"
height="2.7944444444444443in"}

![](media/image14.png){width="6.268055555555556in"
height="2.7645833333333334in"}

![](media/image15.png){width="6.268055555555556in" height="2.8in"}

![](media/image16.png){width="6.268055555555556in"
height="2.7868055555555555in"}

![](media/image17.png){width="6.268055555555556in" height="2.81875in"}

![](media/image18.png){width="6.268055555555556in"
height="2.801388888888889in"}

![](media/image19.png){width="6.268055555555556in"
height="2.7784722222222222in"}

**\
**

Project Work on

***“Pizza Chatbot Development”***

Using

***Azure QnA Maker Service***

***Chapter -II***

![](media/image1.png){width="2.3in" height="0.5in"}

Submitted by

***Sasidhara Kashyap Chaturvedula***

**Second year B. Tech, GRIET, Hyderabad**

Submitted to

***Future Ready Talent***

![](media/image2.png){width="1.5083333333333333in"
height="0.7166666666666667in"}**\
**

**Microsoft Azure Bot Framework Architecture**
==============================================

![](media/image20.png){width="6.625in" height="9.239583333333334in"}**\
**

**Microsoft Azure QnA Maker Development Cycle**
===============================================

![](media/image21.png){width="6.268055555555556in"
height="5.497222222222222in"}

**Life Cycle of a Conversational Bot**
======================================

![](media/image22.png){width="6.268055555555556in"
height="1.1347222222222222in"}

**How to build a bot**
----------------------

Azure Bot Service and the Bot Framework offer an integrated set of tools
and services to facilitate the building process. Choose your favorite
development environment or command line tools to create your bot. SDKs
exist for C\#, Java, JavaScript, Typescript, and Python. We provide
tools for various stages of bot development to help you design and build
bots.

### **Plan**

As with any type of software, having a thorough understanding of the
goals, processes and user needs is important to the process of creating
a successful bot. Before writing code, review the bot [design
guidelines](https://docs.microsoft.com/en-us/azure/bot-service/bot-service-design-principles?view=azure-bot-service-4.0) for
best practices and identify the needs for your bot. You can create a
simple bot or include more sophisticated capabilities such as speech,
natural language understanding, and question answering.

### **Build**

Your bot is a web service that implements a conversational interface and
communicates with the Bot Framework Service to send and receive messages
and events. Bot Framework Service is one of the components of the Azure
Bot Service and Bot Framework. You can create bots in any number of
environments and languages.

![](media/image23.png){width="6.291666666666667in"
height="2.8229166666666665in"}

### **Test**

Bots are complex apps with a lot of various parts working together. Like
any other complex app, this can lead to some interesting bugs or cause
your bot to behave differently than expected. Before publishing, test
your bot. We provide several ways to test bots before they are released
for use:

-   Test your bot locally with
    > the [emulator](https://docs.microsoft.com/en-us/azure/bot-service/bot-service-debug-emulator?view=azure-bot-service-4.0).
    > The Bot Framework Emulator is a stand-alone app that not only
    > provides a chat interface but also debugging and interrogation
    > tools to help understand how and why your bot does what it does.
    > The Emulator can be run locally alongside your in-development
    > bot application.

-   Test your bot on
    > the [web](https://docs.microsoft.com/en-us/azure/bot-service/bot-service-manage-test-webchat?view=azure-bot-service-4.0).
    > Once configured through the Azure portal your bot can also be
    > reached through a web chat interface. The web chat interface is a
    > fantastic way to grant access to your bot to testers and other
    > people who do not have direct access to the bot's running code.

### **Publish**

When you are ready for your bot to be available on the web, publish your
bot
to [Azure](https://docs.microsoft.com/en-us/azure/bot-service/bot-builder-howto-deploy-azure?view=azure-bot-service-4.0) or
to your own web service or data center. Having an address on the public
internet is the first step to your bot coming to life on your site, or
inside chat channels.

### **Connect**

Connect your bot to channels such as Facebook, Messenger, Kik, Slack,
Microsoft Teams, Telegram, text/SMS, and Twilio. Bot Framework does most
of the work necessary to send and receive messages from all these
different platforms - your bot application receives a unified,
normalized stream of messages regardless of the number and type of
channels it is connected to. For information on adding channels,
see [channels](https://docs.microsoft.com/en-us/azure/bot-service/bot-service-manage-channels?view=azure-bot-service-4.0) topic.

### **Evaluate**

Use the data collected in Azure portal to identify opportunities to
improve the capabilities and performance of your bot. You can get
service-level and instrumentation data like traffic, latency, and
integrations. Analytics also provides conversation-level reporting on
user, message, and channel data

**Decision Making Between LUIS and QnA Maker**
==============================================

**When to use the QnA Maker?**\
If your organization has lots of static questions and answers
(Example: [Questions/Answers
Sample](https://www.defense.gov/ask-us/listing/)), take advantage of out
of the box features of QnA Maker. Upload your static questions and
answers into QnA Maker Portal, and your application can call QnA API to
search for questions asked by the user on the front-end application and
return the response.

**When to use the LUIS?**\
If you would like to design the application which needs to extract the
information from the user’s questions and further process their intents,
then use the LUIS.

**Process**
===========

***README.md*** file given in GitHub has the required information and
some of the screenshots below.

![](media/image24.png){width="6.268055555555556in"
height="2.810416666666667in"}

**Task 1**
==========

-   **Create a Resource Group on Azure**
    ====================================

    ![](media/image25.png){width="6.268055555555556in"
    height="2.7895833333333333in"}

**Task 2**
==========

-   **Create a QnA Maker Service on Azure**
    =======================================

![](media/image26.png){width="6.268055555555556in"
height="2.785416666666667in"}

**Task 3**
==========

-   **Create a Knowledge Base on Azure**
    ====================================

![](media/image27.png){width="6.268055555555556in"
height="2.5701388888888888in"}

**Task 4**
==========

-   **Create an App Service on Azure**
    ==================================

![](media/image28.png){width="6.268055555555556in"
height="2.748611111111111in"}

**Task 5**
==========

-   **Create a Web App Bot on Azure**
    =================================

![](media/image29.png){width="6.268055555555556in"
height="2.803472222222222in"}

**Task 6**
==========

-   **Testing my Bot on Azure**
    ===========================

![](media/image30.png){width="6.914483814523185in"
height="1.0194444444444444in"}

![](media/image31.png){width="6.96875in" height="3.367826990376203in"}

![](media/image32.png){width="6.875in" height="1.3125in"}

![](media/image33.png){width="6.677083333333333in"
height="2.8333333333333335in"}

![](media/image34.png){width="6.802083333333333in" height="4.28125in"}

![](media/image35.png){width="6.447916666666667in" height="4.0in"}

![](media/image36.png){width="6.749194006999125in"
height="5.020833333333333in"}

**EMBEDDED HTML FILE**
======================

&lt;!DOCTYPE html&gt;

&lt;html lang="en"&gt;

&lt;head&gt;

&lt;title&gt;Azure QnA Chatbot&lt;/title&gt;

&lt;meta charset="utf-8"&gt;

&lt;meta name="viewport" content="width=device-width,
initial-scale=1"&gt;

&lt;style&gt;

\* {

box-sizing: border-box;

}

body {

font-family: Arial, Helvetica, sans-serif;

}

/\* Style the header \*/

header {

background-color: \#666;

padding: 30px;

text-align: center;

font-size: 35px;

color: white;

}

/\* Create two columns/boxes that floats next to each other \*/

nav {

float: left;

width: 30%;

height: 300px; /\* only for demonstration, should be removed \*/

background: \#ccc;

padding: 20px;

}

/\* Style the list inside the menu \*/

nav ul {

list-style-type: none;

padding: 0;

}

article {

float: left;

padding: 20px;

width: 70%;

background-color: \#f1f1f1;

height: 300px; /\* only for demonstration, should be removed \*/

}

/\* Clear floats after the columns \*/

section::after {

content: "";

display: table;

clear: both;

}

/\* Style the footer \*/

footer {

background-color: \#777;

padding: 10px;

text-align: center;

color: white;

}

/\* Responsive layout - makes the two columns/boxes stack on top of each
other instead of next to each other, on small screens \*/

@media (max-width: 600px) {

nav, article {

width: 100%;

height: auto;

}

}

&lt;/style&gt;

&lt;/head&gt;

&lt;body&gt;

&lt;iframe src='https://webchat.botframework.com/embed/sasi-bot?s=
Dzo1AMv330s.T-iyevx4LeuSjFC7-zhhwS8fBG2PHmdZazY7sdZASUM'
style='min-width: 400px; width: 100%; min-height:
500px;'&gt;&lt;/iframe&gt;

&lt;/body&gt;

&lt;/html&gt;

**URLs**
========

-   ***GitHub URL:*
    https://github.com/sasidhara-kashyap0903/PizzaBot-azure-master**

<!-- -->

-   ***Demo URL:***
    **https://sites.google.com/view/azurepizzaqnabotcom/home?authuser=0**

**Account IDs**
===============

-   ***Git Hub ID:* sasidhara-kashyap0903**

-   ***Azure Account ID:* <sasidhara.kashyap@gmail.com>**

**Technologies / Tools Used**
=============================

-   ***Microsoft Azure QnA Maker Service***

-   ***Git Hub***

-   ***Microsoft Office***

-   ***Microsoft Visual Studio***

**Expected Outcome**
====================

By the end of this milestone, you would be having a working chatbot
system that orders your favourite food like Pizzas, Cakes, Ice Creams
and Garlic Bread to the user along with chatting and provides you rating
facility how my service went with you.

**Acknowledgements**
====================

My sincere thanks, to Microsoft for an impressive QnA Maker service on
MS Azure Cloud to make the chatbot development easy. It was a wonderful
experience learning this and would like to explore more in next two
years of my B.Tech. Sincere appreciation to Team of Future Ready Talent
who supported and encouraged us to work on this project.
