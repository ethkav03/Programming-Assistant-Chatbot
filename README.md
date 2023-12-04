# Programming Assistant Chatbot
## 1. Introduction
In this report I will give a brief overview of my “Programming Assistant Chatbot”. I will
discuss the research I conducted as well as developmental and creative choices made when
building the application. I will showcase my use of AI API in the project and interesting
features and discoveries made along the way
## 2. Research Conducted
When conducting research for this project, my number one priority was finding an API that
was useful and easy enough for me to learn to implement in a timely fashion. Below is a list
of a few APIs that I looked at in my research.
- **OpenAI GPT:** OpenAI provides various versions of GPT models, including GPT-3.5,
GPT-4 etc. These models are pre-trained on a diverse range of internet text and can
be fine-tuned for various natural language processing (NLP) tasks, such as text
completion, translation, and summarization.
- **Google Cloud Vision API:** This API enables developers to integrate powerful image
analysis capabilities into their applications. It can perform tasks like labelling images,
detecting objects and faces, reading printed and handwritten text, and more.
- **Microsoft Azure Cognitive Services:** Azure Cognitive Services is a suite of APIs
and services that cover various AI capabilities, including computer vision, speech
recognition, language understanding, and decision-making. For example, the
Computer Vision API provides image analysis, while the Speech API converts
spoken language into written text.
- **IBM Watson Natural Language Understanding:** This API allows developers to
extract insights and meaning from unstructured text. It can analyse text for sentiment,
entities, concepts, emotion, and more. It's useful for applications that require
understanding and processing of human language.
- **TensorFlow Serving:** TensorFlow Serving is not an API per se but a system for
serving machine learning models in production. It allows you to deploy trained
models for inference using a standardised API. TensorFlow models, among others,
can be served using this infrastructure.
- **AWS Rekognition:** Amazon Rekognition is a deep learning-based image and video
analysis service. It can identify objects, people, text, scenes, and activities in images
and videos. It's commonly used for applications like facial recognition, content
moderation, and image analysis.
## 3. Chosen API
The API I chose for this assignment was OpenAI. Specifically, GPT-3.5. My reasoning for
using OpenAI, was that I have used it in the past for other smaller personal projects, as well
as there being a plethora of documentation, articles and videos online on how to use it.
GPT-3.5 was the most well suited API for my project as I use its natural language processing
capabilities for this project. It is also cheaper to make requests to GPT-3.5 as opposed to
GPT-4 or one of the other AI models OpenAI provides.
## 4. Overview Of Application
To give a brief overview of the created application, it is a programming assistant chatbot,
which can be used to assist on your programming endeavours. It is loaded with a few basic
commands that can be employed on your provided code. The user also specifies the
programming language, and selects a function to perform.
Built-in functions:
- **‘Add comments to my code.’** - The chatbot will return the user's code with
comments included to explain certain aspects of the provided code.
- **‘Fix my code.’** - The user provides their code which is returning an error of some
kind and the chatbot identifies the issue(s), and suggests fixes.
- **‘Suggest improvements for my code.’** - This function will improve your code for
you. Whether that is rewriting an inefficient algorithm or tidying up the code.
- **‘Translate my code to another language.’** - Users can ask for their code to be
translated to another language. For example Python to Java.
- **‘Write some documentation for my code in markdown.’** - This function will write a
detailed document describing the functionality of the code. THe entire document is
written in markdown.
## 5. Technologies Employed
I used a wide range of technologies to create this application. Many of which I had had
experience with in the past, and others that were new to me and required me to conduct
further research.
- **Development Platform:** For this assignment we were required to build our
application using the Ancient Brain platform. This was covered extensively in our
labs, with plenty of documentation readily available.
- **Programming Language:** Ancient Brain uses JavaScript, so this was quite
convenient as we covered JavaScript last year in our Full STack Development
module. I am quite confident programming in JavaScript.
- **AI API:** OpenAI’s GPT-3.5 as discussed above.
- **CSS Frameworks:** I used Bootstrap for a lot of the CSS in the application. Its
easy-to-use classes allowed me to create a visually appealing page.
## 6. Challenges Faced
I had never used the GPT API for an application like this before. A challenge I faced was to
find the right way of structuring the prompts so that I would get the desired result, but it
would also be dynamic in a sense so that it would apply to many different functions. It was a
relatively easy solution. I was able to construct the prompt in a similar to the following format:\
<function> Language: <language> Code: <code>\
Another problem encounter was parsing text vs code from the returned prompt. The
sequence ``` was the identifier for when the result transitioned from text to code. Initially I
was able to parse out one occurrence of code in the response. However, if it included more
than one code snippet they would be treated as plaintext. To fix this I modified some code
(see Figure 6.1) that I found on a forum for GPT-3.5 API.

Fig 6.1 - Code Snippet [1]
## 7. Interesting Discoveries
At a certain point in development, once a level of functionality had been achieved, I was able
to use the application to debug specific sections of its own code. Resulting in somewhat
semi-self sustainable characteristics.
## 8. Conclusion
In conclusion, the creation of the "Programming Assistant Chatbot" was a dynamic process
involving strategic decisions, creative problem-solving, and the integration of powerful
technologies. The selection of OpenAI's GPT-3.5, supported by extensive documentation,
facilitated smooth integration into the user-friendly chatbot developed on the Ancient Brain
platform using JavaScript and Bootstrap. Despite challenges in structuring prompts and
parsing responses, the iterative refinement process showcased adaptability and commitment
to enhancing functionality. An unexpected discovery was the chatbot's ability to debug its
own code, demonstrating unintended yet intriguing versatility. This project underscores the
synergy of diverse technologies and problem-solving in the ever-evolving landscape of AI,
capturing the technical journey with emphasis on challenges and the continuous pursuit of
innovation in application development.
## 9. References
[1] Extract code from Text gpt response, Available at:
https://community.openai.com/t/extract-code-from-text-gpt-response/27152 (Accessed on
3rd December 2023)