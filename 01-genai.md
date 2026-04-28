# Introduction to generative AI

> what is generative ai
- Generative AI powers applications that can create content, 
answer questions, and assist with tasks. 
- we'll explore the fundamentals of generative AI, 
- including large language models (LLMs), prompts, and AI agents.

## Learning objectives

Describe core concepts of generative AI.
Explain how large language models (LLMs) work.
Consider how to create effective prompts for LLMs.
Describe core concepts of agents and agentic AI solutions.


## Introduction
Generative AI, and technologies that implement it are increasingly in the public consciousness – even among people who don't work in technology roles or have a background in computer science or machine learning. The futurist and novelist Arthur C. Clarke is quoted as observing that "any sufficiently advanced technology is indistinguishable from magic". In the case of generative AI, it does seem to have an almost miraculous ability to produce human-like original content, including poetry, prose, and even computer code.

However, there's no wizardry involved in generative AI – just the application of mathematical techniques incrementally discovered and refined over many years of research into statistics, data science, and machine learning. You can gain a high-level understanding of how the magic trick is done by learning the core concepts and principles explored in this module. As you learn more about the generative AI technologies we have today, and how it powers a new generation of AI agents; you can help society imagine new possibilities for AI tomorrow.
## LLMs
At the core of generative AI, large language models (LLMs) - and their more compact relations, small language models (SLMs) - encapsulate the linguistic and semantic relationships between the words and phrases in a vocabulary. The model can use these relationships to reason over natural language input and generate meaningful and relevant responses.

Fundamentally, LLMs are trained to generate completions based on prompts. Think of them as being super-powerful examples of the predictive text feature on many cellphones. A prompt starts a sequence of text predictions that results in a semantically correct completion. The trick is that the model understands the relationships between words and it can identify which words in the sequence so far are most likely to influence the next one; and use that to predict the most probable continuation of the sequence.

For example, consider the following sentence:

I heard a dog bark loudly at a cat

Now, suppose you only heard the first few words: "I heard a dog ...". You know that some of these words are more helpful clues as to what the next word might be than others. You know that "heard" and "dog" are strong indicators of what comes next, and that helps you narrow down the probabilities. You know that there's a good chance the sentence will continue as "I heard a dog bark".

You're able to guess the next word because:

You have a large vocabulary of words to draw from.
You've learned common linguistic structures, so you know how words relate to one another in meaningful sentences.
You have an understanding of semantic concepts associated with words - you know that something you heard must be a sound of some kind, and you know that there are specific sounds that are made by a dog.
So how do we train a model to have these same abilities?

### Tokenization
The first step is to provide the model with a large vocabulary of words and phrases; and we do mean large. The latest generation of LLMs have vocabularies that consist of hundreds of thousands of tokens, based on large volumes of training data from across the Internet and other sources.

Wait a minute. Tokens?

While we tend to think of language in terms of words, LLMs break down their vocabulary into tokens. Tokens include words, but also sub-words (like the "un" in "unbelievable" and "unlikely"), punctuation, and other commonly used sequences of characters. The first step in training a large language model therefore is to break down the training text into its distinct tokens, and assign a unique integer identifier to each one, like this:

I (1)
heard (2)
a (3)
dog (4)
bark (5)
loudly (6)
at (7)
a (3) already assigned
cat (8)
and so on.

As you add more training data, more tokens will be added to the vocabulary and assigned identifiers; so you might end up with tokens for words like puppy, skateboard, car, and others.

### Transforming tokens with a transformer
Now that we have a set of tokens with unique IDs, we need to find a way to relate them to one another. To do this, we assign each token a vector (an array of multiple numeric values, like [1, 23, 45]). Each vector has multiple numeric elements or dimensions, and we can use these to encode linguistic and semantic attributes of the token to help provide a great deal of information about what the token means and how it relates to other tokens, in an efficient format.

We need to transform the initial vector representations of the tokens into new vectors with linguistic and semantic characteristics embedded in them, based on the contexts in which they appear in the training data. Because the new vectors have semantic values embedded in them, we call them embeddings.

To accomplish this task, we use a transformer model. This kind of model consists of two "blocks":

An encoder block that creates the embeddings by applying a technique called attention. The attention layer examines each token in turn, and determines how it's influenced by the tokens around it. To make the encoding process more efficient, multi-head attention is used to evaluate multiple elements of the token in parallel and assign weights that can be used to calculate the new vector element values. The results of the attention layer are fed into a fully connected neural network to find the best vector representation of the embedding.
A decoder layer that uses the embeddings calculated by the encoder to determine the next most probable token in a sequence started by a prompt. The decoder also uses attention and a feed-forward neural network to make its predictions.

