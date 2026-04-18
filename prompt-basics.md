# PROPMT ENGINEERING

## prompt-engineering-basics

### intro

- In this chapter,
- you’ll learn the basics of prompt engineering
and how to craft effective prompts to obtain desirable outputs for various tasks.

Prompting is at the heart of working with LLMs.
The prompt provides context for the text that we want the model to generate.
The prompts we create can be anything from simple instructions to more complex pieces of text,
and they are used to encourage the model to produce a specific type of output.

Coming up with a good prompt is a bit of both science and art.
On the one hand,
we know the broad patterns that enable us to construct a prompt that will generate the output that we want. But on the other hand,
there is so much room for creativity and imagination also.

### writing-basic-prompt

The best way to design prompts for a model is to give a command or an instruction.
One way to do this is by using imperative verbs,
for example: generate, write, list, provide, and other variations.

For instance, let’s say that we are creating the product description copy for a wireless earbuds product.

We can write the prompt as follows.
__"Generate a concise product description for the product: wireless earbuds."__

__

RESPONSE

Sure! Here is a concise product description for wireless earbuds:

"Experience unparalleled sound with our wireless earbuds. Immerse yourself in rich, high-quality audio and enjoy the freedom of movement without tangles or hassles. Our earbuds offer a secure and comfortable fit, ensuring they stay put during any activity. With a sleek and portable design, these earbuds are the perfect companion for your active lifestyle."
__

That’s not bad.
With a simple, one-line prompt,
we already have a piece of product description that can make a digital marketer proud!

### Layering Additional Instructions

But perhaps we want to be more specific regarding what we want the output to look like.
For this, we can layer additional instructions onto the model in the prompt.
Let’s say we want the model to write the product description in a particular format with specific information.
In this case, we can append this specific instruction in the prompt.
__
Generate a concise product description for the product: wireless earbuds.
    Use the following format: Hook, Solution, Features and Benefits, Call to Action.
__

RESPONSE

Here is a concise product description for wireless earbuds:

__Hook:__ Tired of tangled cords and restricted movement?

__Solution:__ Go wireless with our latest earbuds!

__Features and Benefits:__

- Sleek and ergonomic design ensures a secure and comfortable fit.
- Advanced Bluetooth technology for seamless connectivity and uninterrupted audio.
- Immersive sound quality with powerful bass and crystal-clear highs.
- Built-in microphone for hands-free calls and voice assistant access.
- Convenient charging case provides on-the-go power.

__Call to Action:__ Experience true wireless freedom and elevate your audio experience with our cutting-edge earbuds. Order now and enjoy uninterrupted music, calls, and more!
The model returns an output following the format that we wanted.

### Adding Context to a Prompt

The prompt can also be constructed as a combination of an instruction and some context.
Let’s see this in action with another example: emails.
We can create a prompt to summarize an email, which is included in the prompt for context.

__
Summarize this email in one sentence.
    Dear [Team Members],
    I am writing to thank you for your hard work and dedication in organizing our recent community meetup. The event was a great success and it would not have been possible without your efforts.
    I am especially grateful for the time and energy you have invested in making this event a reality. Your commitment to ensuring that everything ran smoothly and that our guests had a great time is greatly appreciated.
    I am also thankful for the support and guidance you have provided to me throughout the planning process. Your insights and ideas have been invaluable in ensuring that the event was a success.
    I am confident that our community will benefit greatly from this event and I am excited to see the positive impact it will have.
    Thank you again for your hard work and dedication. I am looking forward to working with you on future events.
    Sincerely,
    [Your Name]
    __

    __
    Response
    The email expresses gratitude to the team members for their hard work, dedication, and guidance in organizing a successful community meetup, and looks forward to future collaborations.
    __

    This instruction–context prompt format is extremely useful 
    as it means that we can supply additional information as context to help ground the model's output. 
    One such example is a question-answering system for, 
    let's say, a company's knowledge base. Given a question (the instruction), 
    the model will only be able to provide accurate answers if provided with the knowledge base (the context).

    ### Extracting Information
    Let's move to another example — an extraction task, 
    which a generative model can do very well. 
    Given context, which in this case is a description of a movie, 
    we want the model to extract the movie title.
    __
    Extract the movie title from the text below.
    Deadpool 2 | Official HD Deadpool's "Wet on Wet" Teaser | 2018
    __

    __
     RESPONSE

Deadpool 2
__

While this example provides a simple illustration of text extraction,
we recommend using the structured generations feature to build robust text extraction applications.

### Rewriting Text

The model is also effective at tasks
that involve taking a piece of text and rewriting it into another format that we need.

Here's an example.
We have a one-line instruction followed by the context,
which in this case is a blog excerpt.
The instruction is to generate a list of frequently asked questions (FAQ) based on the passage,
which involves a mixture of several tasks, such as extraction and rewriting.
__
Given the following text, write down a list of potential frequently asked questions (FAQ), together with the answers.
    The Cohere Platform provides an API for developers and organizations to access cutting-edge LLMs without needing machine learning know-how.
    The platform handles all the complexities of curating massive amounts of text data, model development, distributed training, model serving, and more.
    This means that developers can focus on creating value on the applied side rather than spending time and effort on the capability-building side.

    There are two key types of language processing capabilities that the Cohere Platform provides — text generation and text embedding — and each is served by a different type of model.

    With text generation, we enter a piece of text, or prompt, and get back a stream of text as a completion to the prompt.
    One example is asking the model to write a haiku (the prompt) and getting an originally written haiku in return (the completion).

    With text embedding, we enter a piece of text and get back a list of numbers that represents its semantic meaning (we’ll see what “semantic” means in a section below).
    This is useful for use cases that involve “measuring” what a passage of text represents, for example, in analyzing its sentiment.
    __

    __
    RESPONSE

Here is a list of potential FAQs based on the provided text:

- __Q: What does the Cohere Platform offer to developers and organizations?__
   A: The Cohere Platform offers an API that provides access to advanced Large Language Models (LLMs) without requiring machine learning expertise. It simplifies the process by handling data curation, model development, training, and serving.

- __Q: What are the key language processing capabilities of the Cohere Platform?__
   A: The platform offers two main capabilities: text generation and text embedding. Text generation involves completing a prompt with a stream of generated text, like writing a haiku. Text embedding returns a numerical representation of the semantic meaning of a text input, useful for sentiment analysis and other measurements.

- __Q: How does the Cohere Platform benefit developers?__
   A: Developers can focus on creating valuable applications without getting bogged down by the complexities of building language processing capabilities from scratch. The platform handles the heavy lifting, allowing developers to save time and effort.

- __Q: What is the difference between text generation and text embedding?__
   A: Text generation is about creating new text based on a prompt, like generating a haiku or continuing a story. Text embedding, on the other hand, translates text into a series of numbers that represent its semantic meaning, enabling quantitative analysis and understanding of the text's context.

- __Q: Can I use the Cohere Platform for sentiment analysis?__
   A: Yes, the text embedding capability of the Cohere Platform is particularly useful for sentiment analysis. By converting text into numerical representations, you can quantitatively analyze and understand the sentiment or emotional tone expressed in a given piece of text.

- __Q: Does the Cohere Platform require machine learning expertise to use?__
   A: No, the platform is designed to abstract away the complexities of machine learning. Developers can utilize the API without needing to understand the intricate details of machine learning or natural language processing.

These FAQs aim to address common inquiries that users might have about the Cohere Platform and its language processing capabilities.
__

By now, we can see how versatile our model is at performing various forms of tasks — 
not just freeform text generation, 
but also following instructions, 
working with contextual information, 
summarizing long passages, 
extracting information, 
rewriting text into different formats, and more.

This is just a taste of what kinds of prompts you can design. 
You can keep layering your instructions to be as specific as you want, 
and see the output generated by the model. And there is really no right or wrong way to design a prompt. 
It’s really about applying an idea and continuing to iterate the prompt 
until you get the outcome you are looking for.