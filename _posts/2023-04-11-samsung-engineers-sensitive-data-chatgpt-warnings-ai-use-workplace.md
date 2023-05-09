---
title: Samsung Engineers Feed Sensitive Data to ChatGPT, Sparking Workplace AI Warnings
categories: [Vulnerabilities/Threats]
tags: [samsung,engineers,chatgpt,ai,artificial,intelligence,workplace,warnings,sensitive,data,gpt]
render_with_liquid: false
image: /assets/img/machine-learning.webp
---

> In three separate incidents, engineers at the Korean electronics giant reportedly shared sensitive corporate data with the AI-powered chatbot.

Recent reports about engineers at Samsung Electronics inadvertently leaking sensitive company information via ChatGPT in three separate incidents highlight why policies governing employee use of AI services in the workplace are quickly becoming a must for enterprise organizations.

The Economist Korea, one of the first to report on the data leaks, described the first incident as involving an engineer who pasted buggy source code from a semiconductor database into ChatGPT, with a prompt to the chatbot to fix the errors. In the second instance, an employee wanting to optimize code for identifying defects in certain Samsung equipment pasted that code into ChatGPT. The third leak resulted when an employee asked ChatGPT to generate the minutes of an internal meeting at Samsung.

The incidents played out exactly the same way that researchers have been warning that they could, since OpenAI made ChatGPT publicly available in November. Security analysts have noted how, in all instances where users share data with ChatGPT, the information ends up as training data for the machine learning/large language model (ML/LLM). They have noted how someone could later retrieve the data using the right prompts. 

ChatGPT creator, OpenAI, itself has warned users on the risk: "We are not able to delete specific prompts from your history. Please don't share any sensitive information in your conversations," OpenAI's user guide notes.

### Samsung Enacts Emergency Anti-ChatGPT Measures

The situation has apparently prompted a rethink of ChatGPT use at Samsung after the third incident, just barely three weeks after the South Korean electronics giant allowed employees access to the generative AI tool. The company had initially banned the technology over security and privacy concerns before relenting.

The Economist reported Samsung's emergency measures to limit ChatGPT use internally as including restricting employees from asking questions of ChatGPT that were larger than 1,024 bytes and considering disciplinary action against employees who share corporate data with LLMs such as ChatGPT.

Samsung did not respond to a Dark Reading request seeking clarification on the three incidents and the company's response to them. Security researchers, however, have been warning that such leaks could become common as employees begin leveraging ChatGPT for various use cases within the enterprise.

A study that Cyberhaven conducted earlier this year found many workers at client companies pasting source code, client data, regulated information, and other confidential data into ChatGPT. Examples included an executive who pasted his company's 2023 strategy document into the chatbot so it could generate a PowerPoint slide presentation, and a doctor who entered a patient's name and medical diagnosis so ChatGPT could generate a letter to the patient's insurance company.

### AI: A Risk vs. Benefit Gamble for Enterprises

"From an employee's perspective, ChatGPT-like tools offer the potential to be exponentially more productive, making them hard to ignore," says Krishna Vishnubhotla, vice president of product strategy at Zimperium. However, it's important to consider the risks vs. rewards equation, which will vary depending on specific roles and responsibilities, he notes. For instance, employees working with intellectual property would require more guidance and precautions on how to use tools like ChatGPT he says: "It is crucial for organizations to understand how productivity will look and where it will come from before they embrace this opportunity."

Michael Rinehart, vice president of artificial intelligence at Securiti, says it's important to remember that advanced Generative AI tools such as ChatGPT cannot distinguish between what they should and should not memorize during training. So, organizations that want to harness them for different use cases should consider using tools for classifying, masking, or tokenizing personal and other sensitive data.

Or "a second approach is the use of differential privacy. Differential privacy offers provable protection of individuals in structured data," Rinehart says.

### Differential Privacy

Rinehart describes differential privacy as a technique for protecting data in a dataset. "It involves adding noise — or error — to real data," he says. The synthetic data will have many of the important characteristics of real-world data without exposing the individuals in the dataset. "If used properly, even if the synthetic dataset were leaked, privacy would still be protected. Enterprise-grade synthetic data generators with differential privacy are now available," he says.

Rinehart perceives attempts by organizations to ban ChatGPT use in the workplace as ill conceived and unlikely to work. "A consistent story in the field of security is that it may be better to offer a secure path to using a tool than to block it," he says. "If a tool offers incredibly high benefits, people may attempt to circumvent blocks to take advantage of it."

Melissa Bischoping, director of endpoint security at Tanium, says the issue with sharing data to ChatGPT lies in the fact that the creators can see the data and use it to understand how the model continues to train and grow. Once a user shares information with ChatGPT, that information becomes part of the next model. 

"As organizations want to enable use of powerful tools like ChatGPT, they should explore options that allow them to leverage a privately trained model so their valuable data is only used by their model and not leveraged by iterations on training for the next publicly available model."