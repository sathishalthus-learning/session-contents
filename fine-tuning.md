# fine-tuning
LLMs have been trained to be useful in practical business applications.
you can leverage a pre-trained LLM to build a chatbot that performs tasks ranging from summarization to copywriting to question answering.
Depending on the use case you have in mind, you might want to amend how the LLM generates its output. 
For instance, if your task uses highly technical data 
or you want to change the chatbot’s output format, 
you often need to perform another round of training on additional data to ensure the best performance. 
This extra training is referred to as fine-tuning.

Fine-tuning is also recommended when you want to incorporate your company's unique knowledge base. For example, if you are aiming to use a model to draft responses to customer-support inquiries, fine-tuning on old conversations with customers can improve the quality of the output.

## Step-by-Step Guide
### Step 1: Prepare and Validate the Dataset
- we create a .jsonl where each JSON object is a conversation containing a series of messages.
First, ensure your data is in jsonl format. It should have the following structure:

messages: This contains a list of messages of the conversation
A message consist of the following parts:

role: The current speaker. You can pick from System, User, or Chatbot.
content: This contains the content of the message.
For your dataset, make sure that each line contains one whole example.

### Step 2: Fine-Tune the Model
-We kick off a fine-tuning job by navigating to the fine-tuning tab of the Dashboard. 
- Next, upload the .jsonl file you just created as the training set by clicking on the "TRAINING SET" button. When ready, click on "Review data" to proceed to the next step.
Next, upload the .jsonl file you just created as the training set by clicking on the "TRAINING SET" button. When ready, click on "Review data" to proceed to the next step.
Next, you'll see an estimated cost of fine-tuning, followed by a page where you'll provide a nickname to your model. We used coedit-coherence as the nickname for our model. This page also allows you to provide custom values for the hyperparameters used during training, but we'll keep them at the default values for now.
Once you have filled in a name, click on "Start training" to kick off the fine-tuning process. This will navigate you to a page where you can monitor the status of the model. A model that has finished fine-tuning will show the status as READY.
Step 3: Evaluate the Fine-Tuned Model
Once the model has completed the fine-tuning process, it’s time to evaluate its performance.
When you're ready to use the fine-tuned model, navigate to the API tab. There, you'll see the model ID that you should use when callingco.chat().
Note the fine-tuned model is still able to respond to prompts like “Hello”, “I’m fine. Can I ask you for help with some tasks?”, and “What’s a good time to visit London” instead of strictly following the fine-tuning objective of editing text.

The model also did a good job with context switching; it can hold a conversation when the user switches from friendly greetings, to a request for writing help, to travel planning, and finally back to writing assistance. It can also infer when the user is asking for help with making a text coherent, even if it is not explicitly stated (e.g., “Help me with this one”) or if the request is buried slightly (e.g., with “Could you help me with this please”).



### fine-tuning steps--