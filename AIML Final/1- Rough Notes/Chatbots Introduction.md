## What Is Chatbot ?

- So what exactly is a chatbot? A chatbot is a way to expose a busi‐ ness’s service or data via a natural language interface. 
- It’s important to understand that as an interface, the chatbot is only as good as the underlying service or data. So if - you’re thinking about building a chatbot, first make sure your services and data are solid. 
- How do you know if they’re in good shape? Imagine the service you’re pro‐ viding has a traditional web or mobile interface. Would that still be useful? 
- If the answer is “no,” your service is not ready for a chatbot interface either.
- If built well, chatbots can help your business cut costs and establish additional revenue streams. 
- A virtual customer support agent can reduce head count and exponentially scale your real- time customer support capabilities. 
- A conversational commerce chatbot gives your business a whole new channel on which you can engage with your customers via messaging platforms.

## The Rise Of Chatbots

Chatbots have been around for a long time. \
Twenty years ago, they would only look for a couple of words from a very highly restricted set of commands: 
“Is this correct? Type yes or no.” 
But as you can see from the Georgia Tech story, the chatbots of today look entirely different. 
There are a few reasons why this is happening now, especially in the enterprise: 
- The availability of NLP capabilities discussed in the prior chap‐ ter, and particularly those in the cloud 
- The proliferation of popular messaging platforms such as Slack and Facebook Messenger 
- The push for natural language interfaces 
 
The next several sections will elaborate on each.

### NLP in the cloud

If you’ve read the previ‐ ous chapter or have experience in machine learning, you’ll know that these NLP techniques are not new. The problem has been the difficulty in utilizing them for people outside the research commu‐ nity. Open source solutions have made these methods more accessi‐ ble, but the arrival of cloud APIs, with a superior user experience, has enabled many more enterprises to use this technology. 

### Proliferation of Messaging Platforms
Messaging apps have come to dominate our mobile app usage. Recent data shows they have surpassed social networks in monthly active users. As more users spend time on messaging apps, compa‐ nies are looking at ways to reach users through these channels. It turns out there is a large amount of contextual data buried in these messages. We make dinner plans, inquire about stores, and look to purchase goods. Companies are now looking to help users by embedding chatbots inside message channels to answer questions or assist with various tasks.

### Natural Language Interface 


In most human-machine interactions, users translate their inten‐ tions into a series of keystrokes and button clicks. The machine then responds via pixels on a screen. Wouldn’t it be nice to talk to com‐ puters the way we talk to each other? This desire for natural lan‐ guage interfaces has always been around. In the early days of search engines, people liked Ask Jeeves because it allowed its users to search the web using natural language. Now, the proliferation of devices such as the Amazon Echo has drawn developers toward the idea of a voice-controlled home. After all, home appliances are notorious for their clunky user interfaces, and to replace them with smart agents that we could talk to seems like a much better user experience.


## How To Build A Chatbot

A chatbot has a frontend and a backend. The frontend is the mes‐ saging channel where the chatbot interacts with the user. The back‐ end is the application logic, the persistence stores, and the supporting services.

### The Messaging Channel

There are many messaging channels available. You can leverage an existing one, such as Slack or Facebook Messenger. You can also build your own messaging layer such as a custom website or mobile app. Choosing the right channel depends on how you plan to engage your users. If you’re a bank with a popular mobile app, you should expose your chatbot there. If you’re a small business with an active Facebook page, integrating your chatbot with Facebook Messenger is a good idea.

### The Backend

Let’s first discuss and expand upon one NLP technology in particu‐ lar—text classifiers. It was not until recently that text classifiers became easy to use and available on the cloud. They’re an important part of chatbots. If you were to approach building a customer sup‐ port chatbot from scratch, the task would probably seem over‐ whelming. After all, even in a narrow domain such as customer support, there can still be an intractable number of different requests. How can you have an answer to every single one of them? The key insight is that though customer requests can be expressed in an almost infinite number of ways, the solution space is magnitudes smaller. Here’s a more specific example. When talking to a customer service agent, a customer might say any of the following:

• “How come I can’t log into my account anymore?” 
• “I forgot my password.” 
• “It says my password is incorrect.” 
• “I’m locked out of my account.”


Luckily, all these requests have the same solution, which is to reset the customer password. So the core functionality of a chatbot is to map all possible user inputs into a much smaller set of responses. This type of pattern recognition is what text classifiers do best. 

Dr. Goel reached the same conclusion when building Jill Watson: “One of the secrets of online classes is that the number of questions increases if you have more students, but the number of different questions doesn’t really go up. Students tend to ask the same questions over and over again.”


#### Using A Framework Vs Building Your Own

The first significant decision in building a chatbot backend is to decide whether to leverage an existing framework. 
There are pros and cons to using one, and if chosen correctly, a framework can provide a large part of the solution with little effort.
But this also means giving up control to the framework itself.
It’s straightforward to build a chatbot within it, but impossible to customize or integrate the chatbot in a way outside the design of the framework.
There are many chatbot frameworks available, including Google Cloud Dialogflow, Wit.ai, Microsoft Bot Framework, Amazon Lex, and IBM Watson Assistant.

#### Anatomy of a Chatbot Backend

If you decide to use a framework, your chatbot’s backend will most likely consist of three main parts: intents, entities, and dialog. These can then be integrated with one or more messaging channels. Extra features such as sentiment analysis, human intervention, or personality can be added as well. 

**Intent**: You usually start building a chatbot with intents. An intent is the purpose of a user’s input. This can be a question about your business hours or a complaint about the registration process. The response of your chatbot to this intent is entirely up to you. It might be a paragraph that answers the question or an action such as starting the password reset process. Another way to think about intents is that they’re the verbs for your chatbots to act on. They dictate what your chatbots will do next.

To train your chatbot to recognize an intent, first determine the action you’d like to map to this intent—for example, provide information on business hours. Then supply the framework with exam‐ ples of user inputs that would require this action. The business hours scenario would include example inputs such as the following:

“What time are you open?” “Are you open on weekends?” “I can’t find your hours of operation.” Usually, a minimum of five inputs is needed, but more is better. Remember, it might be tempting to make up these examples, but it is always better to draw from past data. The more similar these examples are to real-world user requests, the better your chatbot will perform. Typically, an intent (really a text classifier) is built from these examples, so the service will recognize similar inputs in the future, even if they’re not exact matches.

**Entities**: If intents are the verbs for a chatbot to act on, then entities are the nouns. They’re the keywords in a user’s input. If a particular word differentiates one input from another, it probably should be an entity. For example, if a user wants to find the business hours of a bank’s branch, the bank’s location would be one of the entities. Specifically, if a user asks, “What are the hours for the Austin branch?” provide business hours would be the intent, and Austin would be the entity.

**Dialog**: Dialog is the conversation flow. It’s usually represented as a directed graph where each node represents one exchange in the con‐ versation. Together, it is the combined structure of all your possible conversations. Since this can become quite complex, most chatbot platforms provide a UI to help you visualize the process.

**Context Variable**: A context variable contains the information shared between the framework and your application. It’s the way to exchange information between your business logic and the frame‐ work. For example, Watson Assistant provides a context object that lets you store any key/value pair as context variables.

**Human in the loop**: Embedding a human into your chatbot has two significant benefits. First, humans are an excellent way to bootstrap your chatbot before it gathers enough data to operate autonomously. If the chatbot is not confident about its response, it can ask the human for approval or edits before sending it to the end user. Another setup is to have the chatbot provide multiple responses, and have the human choose the most appropriate one.

The second benefit is that humans are the best way to prevent your chatbot from utterly failing your users. There are a few ways to detect if the conversation needs to be routed to a human: 
- The chatbot doesn’t understand the user’s input—this usually means the user input doesn’t match any of your established intents. 
- The conversation is taking too long, or a circular pattern is detected. 
- Negative sentiment is caught in the user’s input. 
- The user directly asks to talk to a real person. 

While seemingly counterintuitive when discussing AI, adding a human to your chatbot process ensures more seamless interactions with your users.


## Challenges of Building A Successful Chatbot

There are many things to get right for a chatbot to be useful. One of the most important is to define the project scope correctly. It needs to be broad enough for the chatbot to be helpful, yet narrow enough so that you’re not wasting time building artificial general intelligence. Specifically, this means capturing as many user requests as possible, yet still reconciling the nuanced differences between each one.

This is not an easy problem. For example, one travel agency tried to deploy a vacation planning chatbot. A critical component was a vocabulary base large enough to recognize all the destinations and their everyday variations. It turns out there were over ten ways people could refer to the Cayman Islands, even assuming all spellings were correct. It took the company months to build a list that could confidently capture all the variations for this one destination.

> It takes at least six months to create a chatbot that’s useful, so make sure to give yourself or your development team enough of a runway.

Unfortunately, there’s not a one-size-fits-all solution. Your best option is to put the chatbot in front of real customers and iterate through user feedback. If you’re a product manager or developer, this should sound familiar. Keep in mind that chatbots are still a nascent field in the enterprise, so you’ll likely be a trailblazer. Nothing but trial and error will help you discover the problems and edge cases specific to your domain.

## Summary

Remember, it’s easy to get started with chatbots, but it takes patience and hard work to create a truly successful one. Don’t try to develop general intelligence! Define the correct scope for your chatbot and keep in mind that context is vital, as the medium has much less bandwidth for communication. We’ll leave you with this analogy from one of our colleagues. Building a chatbot is much like training a new hire—they probably only know a little on their first day. Still, through coaching and supervision, they’ll eventually become a pro‐ ductive employee. It’s essential for your users to see your chatbot as a human, but it’s equally crucial for you to do the same. In the next chapter, we’ll switch gears and talk about computer vision.