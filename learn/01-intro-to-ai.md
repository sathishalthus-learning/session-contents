# Intro to AI Concepts

> 2 minutes

Welcome!

You're presumably here because you want to learn more about artificial intelligence (AI). Maybe you've heard about AI in the media and want to know more; or maybe you're going to be adopting AI at work or in school, and want to know more about what to expect.

This training module is designed to provide a high-level overview of some core capabilities of artificial intelligence (AI) and give you an intuition of how they work. It's not a deeply technical module, and we won't be writing any code or getting into the mathematical details of the machine learning models on which AI is built. Instead, we'll focus on understanding the kinds of things that AI can do, and the basic principles on which it's based.

So, let's go! Move on to the next unit and we'll start our exploration of AI.

> 3 minutes

## Generative AI and agents
Generative AI is a branch of AI that enables software applications to generate new content; often natural language dialogs, but also images, video, code, and other formats.

*For example, a computing history web site could provide a generative AI chat interface into which users can enter questions about key figures, technologies, and events in the history of computing.*

The ability to chat with the site and have it generate original responses to questions creates a compelling interactive experience for users.

### How does generative AI work?
The ability to generate content is based on a language model, which has been trained with huge volumes of data - often documents from the Internet or other public sources of information.

Users interact with generative AI language models through prompts - natural language statements of questions. The language model in a generative AI solution uses the prompt to initiate the generation of a meaningful response.

Generative AI models encapsulate semantic relationships between language elements (that's a fancy way of saying that the models "know" how words relate to one another), and that's what enables them to generate a meaningful sequence of text.

There are large language models (LLMs) and small language models (SLMs) - the difference is based on the volume of data and the number of variables in the model. LLMs are powerful and generalize well, but can be more costly to train and use. SLMs tend to work well in scenarios that are more focused on specific topic areas or that require easily deployed small models for local applications and agents on devices.


### What are agents?

Agents are software applications built on generative AI that can reason over and generate natural language, automate tasks by using tools, and respond to contextual conditions to take appropriate action.

AI agents have three key elements:

A large language model: This is the agent's brain; using generative AI for language understanding and reasoning.
Instructions: A system prompt that defines the agent’s role and behavior. Think of it as the agent’s job description.
Tools: These are what the agent uses to interact with the world. Tools can include:
Knowledge tools that provide access to information, like search engines or databases.
Action tools that enable the agent to perform tasks, such as sending emails, updating calendars, or controlling devices.
With these capabilities, AI agents can take on the role of digital assistants that intelligently automate tasks and collaborate with you to work smarter and more efficiently.

### Generative and agentic AI scenarios

Common uses of generative AI and agents include:

Creating chat bots that answer user questions or engage in conversation.
Implementing AI assistants that assist human users by automating tasks.
Creating new documents or other content (often as a starting point for further iterative development)
Automated translation of text between languages.
Summarizing or explaining complex documents.

> 3 minutes

## Text and natural language

Natural language processing (NLP) is a broad term that covers AI models and techniques for making sense of language. NLP is the foundation on which generative AI large language models (LLMs) are built.

The techniques NLP is built on enable text analysis solutions that can analyze and summarize natural language text. For example, the computing history site could enable users to summarize articles about key historical events and extract specific names, places, and dates from them.

### Text analysis techniques
While many natural language processing scenarios are handled by generative AI models today, there are common text analysis use cases where specialist NLP tools are used to produce predictable results or apply custom rules.

Language detection - determining which language (or languages) a document is written in. Language detection is often the first step in a multi-stage text processing workflow.
Text classification - assigning document to a specific category; including sentiment analysis to determine whether a body of text is positive, negative, or neutral.
Key-term extraction and entity detection - identifying key words or phrases in a document, and finding mentions of entities like people, places, and organizations. A particularly specialized form of entity detection is to detect and redact personally identifiable information (PII); such as names, addresses, telephone numbers, and other private details.
Summarization - Reducing the volume of text while still encapsulating the main points.

### Text analysis scenarios

Common uses of NLP technologies for text analysis include:

Analyzing document or transcripts of calls and meetings to determine key subjects and identify specific mentions of people, places, organizations, products, or other entities.
Analyzing social media posts, product reviews, or articles to evaluate sentiment and opinion.
Implementing chatbots that can answer frequently asked questions or orchestrate predictable conversational dialogs that don't require the complexity of generative AI.
Redacting PII before sharing or analyzing data to comply with privacy policies and legislation.

> 3 minutes

## Speech

Speech capabilities in AI applications and agents enable users to interact with them through spoken language.

For example, our computing history site could include a microphone button that allows users to ask questions verbally, and respond by synthesizing spoken answers.

### Speech recognition

Speech recognition is the ability of AI to "hear" and interpret speech. Usually this capability takes the form of speech-to-text (where the audio signal for the speech is transcribed into text).

### Speech synthesis
Speech synthesis is the ability of AI to vocalize words as spoken language. Usually this capability takes the form of text-to-speech in which information in text format is converted into an audible signal.

AI speech technology is evolving rapidly to handle challenges like ignoring background noise, detecting interruptions, and generating increasingly expressive and human-like voices.

### AI speech scenarios

Common uses of AI speech technologies include:

AI agents that understand spoken input, perform tasks, and respond with spoken results.
Automated transcription of calls or meetings.
Automating audio descriptions of video or text.
Automated speech translation between languages.

> 3 minutes

## Computer vision
 
For example, we could extend the computing history site to enable users to upload images of vintage computers, which can be analyzed, identified, and described.

### How does computer vision work?

There are multiple types of computer vision model.

Image classification is a form of computer vision in which a model is trained with images that are labeled with the main subject of the image (in other words, what it's an image of) so that it can analyze unlabeled images and predict the most appropriate label - identifying the subject of the image.
Object detection is a form of computer vision in which the model is trained to identify the location of specific objects in an image.
Semantic segmentation is an advanced form of object detection where, rather than indicate an object's location by drawing a box around it, the model can identify the individual pixels in the image that belong to a particular object.
Multi-modal models combine visual features and associated text descriptions, enabling them to generate comprehensive descriptions of images.

### Computer vision scenarios

Common uses of computer vision include:

Ai agents that can interpret visual input.
Auto-captioning or tag-generation for photographs.
Visual search.
Monitoring stock levels or identifying items for checkout in retail scenarios.
Security video monitoring.
Authentication through facial recognition.
Robotics and self-driving vehicles.

> 3 minutes

## Information extraction

AI is commonly used to automate information extraction solutions that find information and unlock insights in unstructured data sources, such as scanned documents and forms, images, and audio or video recordings.

For example, we could extend the computer vision capabilities of the computing history application to extract serial numbers and other text from images of computer components and use the information to identify the source computer.

### How does information extraction work?

The basis for most document analysis solutions is a computer vision technology called optical character recognition (OCR), which can identify the location of text in an image. OCR is often combined with an analytical model that can interpret individual values in the document, and so extract specific fields. For example, to match text extracted from a receipt to fields in an expense claim submission.

While most data extraction models have historically focused on extracting fields from text-based forms, more advanced models that can extract information from audio recording, images, and videos are becoming more readily available.

### Data and insight extraction scenarios

Common uses of AI to extract data and insights include:

Automated processing of forms and other documents in a business process - for example, processing an expense claim.
Large-scale digitization of data from paper forms. For example, scanning and archiving census records.
Indexing documents for search.
Identifying key points and follow-up actions from meeting transcripts or recordings.

> 3 minutes

## Responsible AI

Responsible AI is a term used to describe considerations for building AI systems that include guardrails to mitigate the risk of harmful, illegal, or offensive content generation or automated actions.

For example, our computing history solution should avoid providing information to users that would help or encourage illegal or harmful activity.

Content filters are one way that AI systems mitigate the risk of harmful content generation; but a responsible AI solution requires consideration of key principles from its conception, through its design and implementation, and into its operation.

### Principles of responsible AI

Principle	Description
Diagram representing fairness.
Fairness	AI models are trained using data, which is generally sourced and selected by humans. There's substantial risk that the data selection criteria, or the data itself reflects unconscious bias that may cause a model to produce discriminatory outputs. AI developers need to take care to minimize bias in training data and test AI systems for fairness.
Diagram representing reliability and safety.
Reliability and safety	AI is based on probabilistic models, it is not infallible. AI-powered applications need to take this into account and mitigate risks accordingly.
Diagram representing privacy and security.
Privacy and security	Models are trained using data, which may include personal information. AI developers have a responsibility to ensure that the training data is kept secure, and that the trained models themselves can't be used to reveal private personal or organizational details.
Diagram representing inclusiveness.
Inclusiveness	The potential of AI to improve lives and drive success should be open to everyone. AI developers should strive to ensure that their solutions don't exclude some users.
Diagram representing transparency.
Transparency	AI can sometimes seem like "magic", but it's important to make users aware of how the system works and any potential limitations it may have.
Diagram representing accountability.
Accountability	Ultimately, the people and organizations that develop and distribute AI solutions are accountable for their actions. It's important for organizations developing AI models and applications to define and apply a framework of governance to help ensure that they apply responsible AI principles to their work.

### Responsible AI examples
An AI-powered college admissions system should be tested to ensure it evaluates all applications fairly, taking into account relevant academic criteria but avoiding unfounded discrimination based on irrelevant demographic factors.
An AI-powered robotic solution that uses computer vision to detect objects should avoid unintentional harm or damage. One way to accomplish this goal is to use probability values to determine "confidence" in object identification before interacting with physical objects, and avoid any action if the confidence level is below a specific threshold.
A facial identification system used in an airport or other secure area should delete personal images that are used for temporary access as soon as they're no longer required. Additionally, safeguards should prevent the images being made accessible to operators or users who have no need to view them.
An AI agent that offers speech-based interaction should also generate text captions to avoid making the system unusable for users with a hearing impairment.
A bank that uses an AI-based loan-approval application should disclose the use of AI, and describe features of the data on which it was trained (without revealing confidential information).

## Excercises

Explore a generative AI model
Generative AI uses large language models (LLMs) to user prompts.

When the application is ready, use the chat interface to enter the question Who was Ada Lovelace? and review the responses returned by the agent.

Screenshot of the Computing History chat interface.

Note: Responses in the browser-based application may be slow, and might contain inaccuracies.

Enter the follow-up prompt Tell me more about her work with Charles Babbage. and view the response. The conversation should retain the context of previous messages (so “her” is interpreted as Ada Lovelace).
Use the Restart conversation (💬) button to clear the conversation history. Then enter a new prompt: Tell me about the ELIZA chatbot.
Enter a follow-up prompt: How does it compare to modern large language models?

Suggestions for other prompts to try:

Who was Alan Turing?
What was ENIAC?
Tell me about Grace Hopper.
Explore an agent with tools
Agents are generative AI applications that go beyond basic chat functionality and support the use of tools to retrieve knowledge outside of the model’s training data as well as to automate tasks.

In the Computing History app, use the Restart conversation (💬) button to clear the conversation history.
Use the View agent configuration (📃) button to view the agent configuration details, which consist of:
A model with which to reason and generate text.
Instructions to guide behavior and expected functionality.
Tools with which to retrieve knowledge or perform tasks.
Note that the Computing History agent has a web_search tool, which enables it to search the web for knowledge required to answer user questions.

Enter the prompt Search for "Commodore 64". and view the response, which should include links to search results; obtained by the web_search tool.
Now try Shop for a Commodore 64. and view the response.

Note: The application identifies prompts that contain keywords like “search”, “find”, “buy”, or “shop”, and responds with an appropriate search URL for bing.com.

Suggestions for other prompts to try:

Find a vintage computer store in Seattle.
Search for classic Microsoft logos.
Help me buy a PS/2 mouse for an old PC.
Explore text analysis
Text analysis is a subset of natural language processing, in which AI can apply various analytical techniques to summarize, categorize, and extract details from text.

In the Computing history application, use the Restart conversation (💬) button to clear the conversation history.
Paste or type the following prompt (use SHIFT+ENTER to create a new line if typing):

code
 Summarize the following text, and then list the key people, places, and dates it references:
    
 Artificial intelligence (AI) has evolved through several pivotal eras shaped by visionary pioneers, technological breakthroughs, and shifting research priorities. Its conceptual foundations emerged in the 1940s and 1950s, when early thinkers such as Alan Turing, Claude Shannon, Norbert Wiener, Warren McCulloch, and Walter Pitts explored computation, information theory, and the first models of neural networks. In 1950, Turing proposed the influential Turing Test as a criterion for machine intelligence.

 The field formally launched in 1956 at the Dartmouth Conference, organized by John McCarthy, who coined the term “artificial intelligence.” The following decades—often called the Golden Age of AI—saw major advances in symbolic reasoning, early problem‑solving programs, and robotics. Researchers such as Allen Newell, Herbert Simon, and Marvin Minsky pushed the boundaries of what machines could reason about.

 After cycles of inflated expectations and funding declines known as the AI winters (mid‑1970s and late 1980s), progress accelerated again in the 1990s with improved computing power and machine‑learning techniques. Landmark achievements included IBM’s Deep Blue defeating Garry Kasparov in 1997, breakthroughs in probabilistic reasoning, and the rise of data‑driven learning.
 The 2010s ushered in the deep‑learning revolution, producing systems such as AlphaGo (2016), GPT‑3 (2020), and other large‑scale models that demonstrated unprecedented capabilities in vision, language, and decision‑making. Today’s AI continues to evolve rapidly, integrating neural networks, reinforcement learning, and massive datasets to push the frontier of intelligent systems.
Review the response, which include the results of two common text analysis techniques: summarization and named entity recognition.

Note: The app detects prompts that start with “summarize” and then uses statistical techniques and JavaScript NLP packages to perform an extractive summary and extract entities.

Suggestions for other prompts to try:

code
 Summarize this article, and use named entity recognition to identify people, places, and dates:

 Microsoft was founded on April 4, 1975, by childhood friends Bill Gates (then 19) and Paul Allen (22) after they were inspired by the Altair 8800, one of the first personal computers, featured on the cover of Popular Electronics. They contacted the Altair’s maker, MITS, and successfully developed a version of the BASIC programming language, despite initially not owning the machine themselves. The pair formed a partnership called “Micro‑Soft” in Albuquerque, New Mexico, close to MITS’s headquarters, with the goal of writing software for emerging microcomputers.

 In the late 1970s, Microsoft grew by supplying programming languages to multiple hardware vendors, then relocated to the Seattle area in 1979. A pivotal moment came in 1980 when Microsoft partnered with IBM to provide an operating system for the IBM PC, leading to MS‑DOS and establishing the company’s dominance in personal computing. Gates guided the company’s long-term strategy as CEO, while Allen contributed key technical vision in its early years, setting Microsoft on a path that would reshape the software industry.
Explore computer speech
Speech recognition enables AI to process spoken input, which speech synthesis enables it to vocalize output.

In the Computing History application, use the Restart conversation (💬) button to clear the conversation history.
At the bottom of the chat interface, use the Voice input (🎤) button to initiate speech recognition, allow access to your microphone if prompted, and say “Tell me about computer speech”.

After a moment or two, your spoken prompt should be submitted as a message, and a response returned. The response should then be vocalized using speech synthesis.

Note: Speech support for the browser-based application is based on the Web Speech library that is common in most modern browsers. If Web Speech-based speech recognition fails, a fallback offline speech-to-text speech model is loaded and used. In some cases, the required voices to syntheisze speech may not be present on your computer.

Continue the conversation, using the voice input button to ask questions and listening to the responses.

Suggestions for other prompts to try:

Explain speech recognition
What is a vocoder?
Explore computer vision
Computer vision uses image-based models to enable AI to interpret visual input.

In a new browser tab, download computers.zip from https://aka.ms/computer-images, and extract the zipped archive to your local computer (in any folder).
Return to the Computing history application, and use the Restart conversation (💬) button to clear the conversation history.
At the bottom of the chat interface, use the Attach image (📎) button to select any of the images in the folder you extracted, and enter the prompt Tell me about this.

Review the response. Hopefully the model recognized the computer in the image.

Try attaching a different image with the prompt And this?
Try all of the images in the extracted folder. The accuracy of identification and details may vary (particularly when using the browser-based application).

Note: The app uses a custom image classification model based on MOBILENETV2 to predict the image contents, and then submits the predicted class to the generative AI model to generate a summary of information about it.

Suggestions for other prompts to try:

Use Bing to find and download images of computers (and other items), and try asking the Computing History application to identify them. The image classification model in the browser-based app is trained to recognize the following objects:

Altair 8800
Apple II
Commodore 64
Sinclair ZX Spectrum
Other unidentified computers
Non-computers
Printed circuit boards (PCBs)
Explore information extraction
Information extraction combines multiple AI workloads to analyze content and identify important data values. In this example, we’ll use the Computing History app to analyze photographs of printed circuit boards (PCBs) and try to extract information from them.

In a new browser tab, download pcbs.zip from https://aka.ms/pcb-images, and extract the zipped archive to your local computer (in any folder).
Return to the Computing history application, and use the Restart conversation (💬) button to clear the conversation history.
At the bottom of the chat interface, use the Attach image (📎) button to select pcb-1.png in the folder you extracted, and enter the prompt What can you tell me about this?

Review the response. Hopefully, the Computing History application extracted the part number printed on the board and provided some relevant information.

Note: The app uses its custom image classification model to identify images of printed circuit boards, and a JavaScript package for OCR to extract any text they contain.

Suggestions for other prompts to try:

Try the other PCB images in the folder you extracted with prompts that ask the agent about them, and view the responses.

You can also download images of circuit boards and try them, but the simple OCR implementation used in the browser-based application will likely produce poor results.


Explore safety guardrails
Content safety is an important element of responsible AI. As much as possible, developers of AI apps and agents should try to mitigate the risk of AI-generated content that is potentially harmful, illegal, or offensive.

In the Computing History application, use the Restart conversation (💬) button to clear the conversation history.
Enter the prompt Help me make a plan to steal historic computers. and review the response.

The agent should respond in a way that avoids helping with potentially illegal activity, due to content safety guardrails.

Note: The app implements some simple logic to check for innappropriate terms in the prompt.

Suggestions for other prompts to try:

Try the following prompts:

How can I get away with software theft?
How can I use a computer as a weapon?
Teach me how to hack a bank account.
Summary
In this exercise, you explored common AI workloads in a simple example application. The application’s functionality is limited, and does not reflect the kind of performance or capabilities you can expect in a production quality agent; but it should serve to show the kinds of functionality you can achieve with AI.

## Assesment

1. Which is the most accurate description of generative AI?

Generative AI uses a language model to create original content in response to a prompt.

Generative AI is an older form of AI that's superseded by machine learning.

Generative AI is a complex form of AI that can only be used by specialists such as data scientists.
2. What is an AI agent?

A technology professional who builds AI applications.

Anyone who uses AI applications.

An AI application that can perform tasks on behalf of a user.
3. An AI application reads email aloud to a user. Which AI speech capability is being used?

Speech recognition

Speech synthesis

Sentiment analysis

## Summary

Hopefully, this module gave you an insight into some of the core capabilities of AI, and an intuition into how they work. We explored many areas of AI, including:

Generative AI and agents
Natural language processing (NLP) and text analytics
Speech
Computer vision
Information extraction
Responsible AI

## Following Resources


