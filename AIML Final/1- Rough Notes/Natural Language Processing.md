computer scientists began attempts at using software to process and analyze textual components, sentiment, parts of speech, and the various entities that make up a body of text. Until relatively recently, processing and analyzing language has been quite a challenge.

A 2017 study from IBM reported that 90% of the world’s data had been created in the past two years, and that 80% of that data was unstructured.

Interpreting this unstructured data is quite difficult. In fact, process‐ ing human-generated (not machine) words (or natural language) is considered an AI-hard or AI-complete problem. In other words, it’s a challenge that brings the full effort of AI to bear on the problem and isn’t easily solved by a single algorithm designed for a particular purpose.

## Overview Of NLP

Natural language processing is essentially the ability to take a body of text and extract meaning from it using a computer. While compu‐ tational language is very structured (think XML or JSON) and easily understood by a machine, written words by humans are quite messy and unstructured—meaning when you write about a house, friend, pet, or a phone in a paragraph, there’s no explicit reference that labels each of them as such.

Natural language processing is needed when you wish to mine unstructured data and extract meaningful insight from text. General applications of NLP attempt to identify common entities from a body of text; but when you start working with domain-specific con‐ tent, a custom model needs training.

## Components Of NLP
To understand NLP, we first need to understand the components of its model. Specifically, natural language processing lets you analyze and extract key metadata from text, including entities, relations, concepts, sentiment, and emotion.


### Entities 
Likely the most common use case for natural language processing, entities are the people, places, organizations, and things in your text. In our initial example sentence, we identified several entities in the text—friend, car, and phone.

### Relations

How are entities related? Natural language processing can identify whether there is a relationship between multiple entities and tell the type of relation between them. For example, a “createdBy” relation might connect the entities “iPhone” and “Apple.”

### Concepts

One of NLP’s more magical aspects is extracting general concepts from the body of text that may not explicitly appear in the corpus. This is a potent tool. For example, an analysis of an article about Tesla may return the concepts “electric cars” or “Elon Musk,” even if those terms are not explicitly mentioned in the text.

### Keywords

NLP can identify the important and relevant keywords in your con‐ tent. This allows you to create a base of words from the corpus that are important to the business value you’re trying to drive.

### Semantics Roles

Semantic roles are the subjects, actions, and the objects they act upon in the text. Take the sentence, “Intel bought a company.” In this sentence, the subject is “Intel,” the action is “bought,” and the object is “company.” NLP can parse sentences into these semantic roles for various business uses—for example, determining which companies were acquired last week or receiving notifications any time a particular company launches a product.

### Categories

Categories describe what a piece of content is about at a high level. NLP can analyze text and then place it into a hierarchical taxonomy, providing categories to use in applications. Depending on the content, categories could be sports, finance, travel, comput‐ ing, and so on. Possible applications include placing relevant ads alongside user-generated content on a website or displaying all the articles talking about a particular subject.

### Emotions

Whether you’re trying to understand the emotion conveyed by a post on social media or analyze incoming customer support tickets, detecting emotions in text is extremely valuable. Is the content con‐ veying anger, disgust, fear, joy, or sadness? Emotion detection in NLP will assist in solving this problem.

### Sentiment

Similarly, what is the general sentiment in the content? Is it positive, neutral, or negative? NLP can provide a score as to the level of posi‐ tive or negative sentiment of the text. Again, this proves to be extremely valuable in the context of customer support. This enables continued, automatic understanding of sentiment related to your product. Now that we’ve covered what constitutes natural language process‐ ing, let’s look at some examples to illustrate how NLP is currently used across various industries.

## Enterprise Application Of NLP

## How To Use NLP

There are many solutions for natural language processing. Starting with open source software projects, a few of the more popular include Apache NLP, Stanford CoreNLP, NLTK for Python, and SyntaxNet.

When evaluating whether to build in-house, outsource, or use hos‐ ted APIs, ask yourself the following important question: how much of a core component to your business is artificial intelligence? Your answer can then drive the technical level of expertise required for your enterprise application. For example, if you’re an ecommerce company attempting to add intelligence to your customer support system, it would be more appropriate to start with hosted APIs, as better customer support improves the business but isn’t your core functionality.

> According to McKinsey, these recommendation algorithms produce 35% of Ama‐ zon purchases and 75% of Netflix viewings.

## Training Models
If you develop natural language processing from scratch in your enterprise, you’ll create custom models by default. But when you’re using third-party solutions or open source options, the out-of-the- box solution will cover only the majority of cases, and it will be decidedly non-domain-specific. If you want to improve the accuracy and reliability of your output, you’ll want to create and train a cus‐ tom model. This is especially true if you’re using a third-party service.

While there are various ways to accomplish training a model, the details are beyond the scope of this book, as they vary depending on the particular solution. Using IBM Watson NLU as an example, you can train a custom model using the Watson Knowledge Studio (WKS). WKS is a web- based tool that enables domain experts to train a custom natural language processing model without programming. Both developers and non-technical end users can upload relevant documents and then annotate them for their domain-specific entities and relations. They can then use this data to train a custom model via machine learning and publish it to the Watson NLU APIs for use in their applications.


## Challenges Of NLP

First, natural language processing works best with massive data sets: the more data, the better the accuracy. While the data set’s necessary size depends on the actual application, more data is better in general.

(Train This On A Random GC Just For Fun LMFAOOO)

Second, natural language processing isn’t a magic bullet. After you’ve been exploring and working on NLP some, it’s easy to think you’ll obtain easy answers to questions. When you’re testing out NLP, the results tend to be very accurate, as the tendency is to input relatively straightforward bodies of text for testing. Unfortunately, human languages have many nuances. Think of all the phrases and words that are open to interpretation. Concepts like sarcasm are still quite hard to understand via natural language processing. Slang, jar‐ gon, and humor are hard to process as well. 

There’s a tremendous amount of ambiguity in language that is only understood from the context. Additionally, handling spelling mistakes and errors in grammar is especially tricky.

What’s the best way to handle these challenges then? Until the tech‐ nology catches up and increases accuracy in these cases, the best approach is to know they exist and filter/review the content going through natural language processing as much as possible. While this isn’t an optimal solution in and of itself, paying attention to your preprocessed content beforehand and filtering any questionable content in advance is the best option.

## Summary

Natural language processing is a powerful tool used in a wide range of enterprise applications. Since text appears almost everywhere, NLP provides an essential building block for all enterprise applica‐ tions utilizing artificial intelligence. 

In this vein, natural language processing also forms the backbone for creating conversational applications, more commonly known as chatbots. In the next chapter, we’ll discuss these in more detail.