# Week 01 — Assignment Questions

## Q1. AI, Machine Learning, Deep Learning, Generative AI, and AI Agents

### A — Answer

**1. Artificial Intelligence (AI)**

Artificial Intelligence is a field of computer science focused on creating systems that can perform tasks requiring capabilities such as learning, reasoning, recognizing patterns, understanding language, or making decisions.

*Example:* A phone using face recognition to unlock the screen.

**2. Machine Learning (ML)**

Machine Learning is a branch of AI in which a computer learns patterns from data to make predictions or decisions rather than relying only on manually written rules.

*Example:* An email service learning to identify spam messages from examples of spam and legitimate emails.

**3. Deep Learning (DL)**

Deep Learning is a type of Machine Learning that uses neural networks with multiple layers to learn complex patterns from data.

*Example:* A system recognizing objects such as cars, people, and traffic signs in images.

**4. Generative AI**

Generative AI refers to AI systems that create new content, such as text, images, audio, video, or code, based on patterns learned during training.

*Example:* An AI assistant drafting an email from a user's instructions.

**5. AI Agent**

An AI agent is a system designed to pursue a goal by using an AI model and, when needed, tools or actions to gather information, perform tasks, and respond to results.

*Example:* A travel-planning agent that searches for transport options, compares choices, and prepares an itinerary.

### Concept Map

```text
Artificial Intelligence (AI)
          |
          └── Machine Learning (ML)
                    |
                    └── Deep Learning (DL)
                              |
                              └── Many modern
                                  Generative AI systems

AI Agent:
Goal + AI Model + Tools/Actions + Workflow
```

This is a simplified concept map. Generative AI is not limited to one specific model design, and an AI agent is a system or workflow rather than simply another level in the hierarchy.

### How the Concepts Are Related

AI is the broad field. Machine Learning is one approach within AI, and Deep Learning is a type of Machine Learning. Many modern Generative AI systems use deep-learning models to produce new content. An AI agent may use a generative AI model as its reasoning or language component, along with tools and a workflow to pursue a goal. However, not every AI system generates content, and not every chatbot is an agent.

### E — Evidence

1. IBM, Artificial Intelligence: https://www.ibm.com/think/topics/artificial-intelligence
2. IBM, Machine Learning: https://www.ibm.com/think/topics/machine-learning
3. Google Cloud, Generative AI glossary: https://docs.cloud.google.com/docs/generative-ai/glossary
4. Google Cloud, What are AI agents?: https://cloud.google.com/discover/what-are-ai-agents

### V — Verification

I will review these references and check that they support the definitions and relationships explained above. I will distinguish the broad AI field from the narrower concepts of Machine Learning and Deep Learning. I will also check that the agent example involves a goal and actions or tools, rather than only producing a text response.

### R — Reflection

I learned that AI, Machine Learning, Deep Learning, Generative AI, and AI agents are related but do not mean the same thing. The main distinction I need to remember is that Generative AI creates content, while an agent can use a model and tools to work toward a goal. I should verify important claims using reliable sources instead of trusting an AI-generated explanation automatically.
---

## Q2. Is Everything That Looks Intelligent Actually AI?

### A — Answer

A system does not necessarily use Artificial Intelligence just because it performs a task that appears intelligent. Some systems follow explicitly programmed rules, while others use models that learn patterns from data. To classify a system correctly, we need to understand its implementation or find reliable evidence about how it works.

| Scenario | Classification | Reason |
|---|---|---|
| A calculator evaluates 25 × 16 | Conventional software | It performs a programmed mathematical operation. |
| A temperature controller warns when temperature exceeds 80°C | Rule-based software | It checks a fixed threshold. |
| A spam classifier learns from labelled email examples | Machine Learning | It learns patterns from training data to classify emails. |
| An AI assistant summarizes a document | AI system | It uses an AI model to generate a summary. |
| A navigation app estimates arrival time from traffic and historical data | Not enough information to conclude | It may use AI/ML, conventional algorithms, or both. |

### E — Evidence

The scenarios above are used to distinguish explicit rules from learned patterns. I will consult reliable references on Artificial Intelligence and Machine Learning and look for technical documentation before making claims about how a particular real-world product works.

References:

1. IBM, Artificial Intelligence: https://www.ibm.com/think/topics/artificial-intelligence
2. IBM, Machine Learning: https://www.ibm.com/think/topics/machine-learning

### V — Verification

I checked my understanding using three practice examples. A fan that turns on above a fixed temperature threshold is rule-based software. A spam filter trained on labelled examples is a Machine Learning system. For a navigation app, an ETA alone does not establish whether AI is involved; implementation evidence is needed.

### R — Reflection

I learned that a system's visible output is not enough to prove that it uses AI. A fixed rule can produce useful and intelligent-looking behaviour without Machine Learning. I should avoid claiming that a real-world system uses AI unless reliable evidence supports that conclusion.
---

## Q3. What Happens When We Ask an LLM?

### A — Answer

A Large Language Model (LLM) is an AI model trained on large amounts of text to learn language patterns and generate responses. When a user asks a question, the model processes the prompt and available context, estimates likely next tokens, and generates a response token by token.

**Important terms:**

- **Prompt:** The question or instruction given to the model.
- **Token:** A unit of text, such as a word, part of a word, or punctuation.
- **Context:** Information available to the model when generating a response.
- **Probability:** A measure of how likely a possible next token is according to the model.
- **Next-token prediction:** Estimating the next token and repeating this process to generate text.

### Simplified Flow Diagram

```text
User enters a prompt
        |
        v
Text is split into tokens
        |
        v
Model processes prompt and context
        |
        v
Model estimates likely next tokens
        |
        v
Tokens are generated sequentially
        |
        v
Response is displayed to the user
```

### Training vs Inference

**Training:** The model learns patterns from training data by adjusting its internal parameters.

**Inference:** The trained model processes a prompt and generates an output.

### Why Can an LLM Give an Incorrect Answer?

An LLM generates text based on learned patterns and the available context. A fluent response is not necessarily factually correct. The model may misunderstand a question or generate an unsupported claim. Therefore, important information should be checked against reliable references, such as official documentation, technical datasheets, or authoritative publications.

### E — Evidence

I will use a reliable technical explanation of language models and next-token prediction to support this description. I will also check an authoritative source explaining why generated answers can be inaccurate.

### V — Verification

I checked my understanding with practice questions. A prompt is an instruction given to a model, inference is the use of a trained model to generate an output, and next-token prediction does not guarantee factual correctness. These concepts are consistent with the simplified process described above; I will consult and record the exact references used before final submission.

### R — Reflection

I learned that an LLM does not simply retrieve a guaranteed correct answer for every question. It generates a response using learned patterns and available context. I also learned the difference between training and inference. In future, I will verify important technical claims instead of relying only on how confidently an answer is written.
---

## Q4. AI Hallucination Experiment

### A — Answer

**Objective:** To compare two AI assistants' answers to the same factual technical question and verify their claims against an authoritative source.

**Prompt used:**

"For the Arduino Uno R3, identify the microcontroller, operating voltage, clock speed, Flash memory, and SRAM. Give the exact value for each specification and cite a reliable source. If you are uncertain about any value, say so rather than guessing."

I submitted the same prompt to ChatGPT and Google Gemini.

**Results:**

| Specification | ChatGPT response | Gemini response | Verification result |
|---|---|---|---|
| Microcontroller | ATmega328P | ATmega328P | Correct |
| Operating voltage | 5 V | 5 V | Correct |
| Clock speed | 16 MHz | 16 MHz | Correct |
| Flash memory | 32 KB | 32 KB | Correct |
| SRAM | 2 KB | 2 KB | Correct |
| Bootloader allocation | Approximately 0.5 KB | 0.5 KB | Correct for the standard configuration |

Neither response contained an obvious factual error in the five main specifications. Therefore, this experiment did not identify a clear factual hallucination in those claims.

### E — Evidence

**Primary verification source:** Arduino, Arduino Uno Rev3 official product documentation.

https://store.arduino.cc/products/arduino-uno-rev3

The official specifications list the ATmega328P microcontroller, 5 V operating voltage, 16 MHz clock speed, 32 KB Flash memory with 0.5 KB used by the bootloader, and 2 KB SRAM.

### V — Verification

I compared the specifications stated by both assistants with the official Arduino Uno Rev3 product documentation.

All five main specifications matched the official values. The bootloader allocation also matched the standard configuration listed by Arduino.

I observed a difference in source presentation. ChatGPT provided more explanatory details but did not include direct source URLs in the response I recorded. Gemini referred to Probots for the microcontroller claim while also describing its sources as official documentation. The microcontroller value was nevertheless confirmed by Arduino's official source.

I found no obvious incorrect or contradictory specification in the recorded responses. I did identify a need to verify source quality rather than accepting an assistant's claim that its answer is verified.

### R — Reflection

This experiment taught me that an AI answer can be factually correct while still providing incomplete or unclear source attribution. I should distinguish an incorrect claim from a claim that has not been adequately supported by its citation.

I also learned that an experiment does not have to produce a hallucination to be useful. Comparing two assistants and checking their claims against an authoritative reference helped me understand why independent verification is important. In future, I will check technical specifications against manufacturer documentation before relying on them in engineering work.
---

## Q5. AI Assistant vs Search vs Authoritative Reference

### A — Answer

I compared three approaches for answering the same technical question:

**Question:** What are the operating voltage and clock speed of the Arduino Uno R3?

**1. AI assistant**

I asked ChatGPT for the two specifications and requested a reliable source. It reported an operating voltage of 5 V and a clock speed of 16 MHz. It also explained the difference between operating voltage and recommended external input voltage.

**2. Web search**

I searched Google for the same information. The Google AI Overview reported 5 V operating voltage and 16 MHz clock speed. The results also referred to Arduino documentation and other sources. The AI Overview was convenient, but its claims still needed checking against the original source.

**3. Authoritative reference**

I consulted the official Arduino Uno R3 documentation. The documentation identifies the board's 5 V operating voltage and 16 MHz clock speed. This provided a direct reference for checking the values.

### E — Evidence

- AI assistant response: The recorded ChatGPT response in this experiment.
- Web search evidence: My screenshots of the Google AI Overview and Arduino documentation.
- Official reference: https://store.arduino.cc/products/arduino-uno-rev3

### V — Verification

The AI assistant and Google AI Overview both reported 5 V operating voltage and 16 MHz clock speed. These values agree with the official Arduino Uno R3 specifications.

The AI assistant gave a conversational explanation, while Google presented a summarized answer with source references. The official documentation was the most direct source for verifying the technical values. I learned that search summaries and AI answers should be checked against their original sources.

### R — Reflection

I learned that AI assistants are useful for understanding technical concepts, search engines help locate information, and authoritative references are important for confirming exact specifications. For engineering tasks, I would use AI to help explain a concept, search to find relevant documentation, and the manufacturer's official documentation to verify important values.
---

## Q6. What Is an AI Agent?

### A — Answer

An AI agent is a software system designed to pursue a goal by using an AI model, available tools, and a workflow that can involve multiple steps. It can interpret a request, choose an action, use a tool, examine the result, and decide whether more work is needed.

**Important terms:**

1. **LLM:** A Large Language Model that processes and generates language.
2. **LLM application:** Software built around an LLM, potentially with instructions, an interface, and other features.
3. **RAG system:** Retrieval-Augmented Generation retrieves relevant information from a knowledge source and supplies it to a model to help generate a grounded response.
4. **Tool-using assistant:** An assistant that can invoke tools such as a search engine, calculator, or database.
5. **AI agent:** A goal-oriented system that can coordinate reasoning, tools, and multiple steps to complete a task.

### Architecture Diagram

```text
User provides a goal
        |
        v
AI model interprets and plans
        |
        v
Tool call (search, calculator, API)
        |
        v
Tool result returned to the model
        |
        v
Decision: continue or finish?
        |
        +---- Continue: select another action
        |
        v
Final response to the user
```

The agent may repeat the action and result steps when more work is needed.

### AI Agent vs Ordinary Chatbot

An ordinary chatbot may mainly generate a response to a user's message. An AI agent is designed to work toward a goal by selecting actions, using available tools, and responding to the results. Some chatbots also have tools, so the difference depends on the system's design and workflow rather than its name alone.

### Non-VLSI Example: Student Study-Planning Agent

A study-planning agent could ask for an exam date, read the subject list, use a calendar tool to distribute study sessions, check the available time, and present a schedule for the student to review. This illustrates how an agent can combine a goal, tools, and several steps to produce a useful result.

### E — Evidence

Google Cloud, Core concepts of AI agents:

https://cloud.google.com/resources/core-concepts-ai-agents

Google for Developers, Machine Learning Glossary — Agentic:

https://developers.google.com/machine-learning/glossary/agent

These references describe agent components and the use of reasoning, tools, and actions to pursue goals.

### V — Verification

I will review the references to verify the distinction between an LLM, a tool-using application, and an AI agent. I will check that my architecture diagram includes the tool call, returned result, and decision about whether to continue or finish. The study-planning example is an illustrative workflow, not a claim that I built or tested a working agent.

### R — Reflection

I learned that an AI agent is not just a model that generates text. It is a system organized around a goal and may use tools and feedback across several steps. I also learned that not every chatbot is an agent, and a system's actual capabilities depend on its connected tools and workflow.
---

## Q7. Where Should Humans Still Decide?

### A — Answer

AI can help read documents, answer questions, summarize information, generate text, and suggest actions. However, its output may be incomplete, inaccurate, or unsuitable for a particular situation. Human review is important when the consequences of an error are significant.

| AI task | Possible failure | Verification evidence | Who should approve? |
|---|---|---|---|
| Reading a document | An important condition or exception is missed | Compare the output with the original document | The person responsible for using the document |
| Answering a question | An incorrect or unsupported fact is presented | Reliable references or official documentation | The person relying on the answer |
| Summarizing information | Important context is omitted or meaning is changed | Check key statements against the original material | The reader or report owner |
| Generating text | Invented details, incorrect figures, or inappropriate wording | Check facts, names, figures, and intended meaning | The person sending or publishing the text |
| Suggesting an action | Safety risks, constraints, or consequences are overlooked | Evidence, requirements, risk checks, and applicable procedures | The authorized person responsible for the action |

### E — Evidence

For each situation, the relevant evidence depends on the task. Examples include original documents, official technical documentation, verified data, organizational procedures, and safety requirements.

For this question, the table presents a reasoned analysis of potential AI failures and appropriate human oversight. These are illustrative scenarios rather than results of a practical experiment.

### V — Verification

I would verify an AI-generated summary against its original document, check factual answers against reliable references, and review generated text before sending it. For recommendations involving safety or other significant consequences, I would check relevant requirements and seek approval from the qualified or authorized person.

Verification should be appropriate to the risk of the decision. A low-risk draft may need a simple review, while a safety-critical action requires stronger checks.

### R — Reflection

I learned that AI is useful for supporting tasks but should not automatically be treated as the final authority. A human reviewer must consider the evidence, context, risks, and consequences. I would use AI to save time on analysis and drafting while retaining responsibility for decisions that require judgment or authorization.
---

## Q8. Find AI Around You

### A — Answer

I identified five everyday systems that use AI or Machine Learning for particular tasks. I checked public documentation to support the classifications and considered whether a conventional rule-based system could perform a similar task.

| Everyday system | Task type | Evidence of AI use | Could rules do something similar? |
|---|---|---|---|
| Gmail spam detection | Classification | Google's Gmail privacy documentation identifies spam detection as one of its intelligent features. | Yes. Rules can block known senders or flag messages matching fixed criteria, but may be less flexible for unfamiliar spam patterns. |
| Apple Face ID | Recognition and authentication | Apple's security documentation states that Face ID uses neural networks for matching and anti-spoofing. | Simple rules can check a PIN or password, but ordinary fixed rules cannot perform the same learned facial matching by themselves. |
| Google Maps traffic prediction | Prediction | Google documents the use of machine learning with historical traffic patterns and live traffic conditions. | Fixed speed assumptions and predefined rules can estimate travel time, but may not adapt as effectively to changing traffic patterns. |
| Spotify recommendations | Recommendation | Spotify's AI research documentation describes AI and Machine Learning for recommendations and content discovery. | Fixed playlists or manually written rules can recommend items, but may not provide the same personalized recommendations. |
| Google Assistant speech recognition | Speech recognition | Google documents the use of deep neural networks in speech-recognition technologies used by Google Assistant. | Fixed voice commands can recognize a limited set of predefined patterns, but learned speech models can handle more variation. |

### E — Evidence

1. Google, Gmail privacy and spam detection: https://support.google.com/mail/answer/10434152
2. Apple, Platform Security: https://help.apple.com/pdf/security/en_US/apple-platform-security-guide.pdf
3. Google, How AI helps predict traffic and determine routes: https://blog.google/products-and-platforms/products/maps/google-maps-101-how-ai-helps-predict-traffic-and-determine-routes/
4. Spotify Research, Artificial Intelligence: https://research.atspotify.com/artificial-intelligence
5. Google Assistant Help, Learn how Google improves speech models: https://support.google.com/assistant/answer/11140942

### V — Verification

I used public documentation from the companies responsible for these services to check whether AI or Machine Learning is used for the specific tasks listed. The documentation supports the examples of spam detection, face recognition, traffic prediction, recommendations, and speech recognition.

I also distinguished between evidence for a particular AI feature and assumptions about an entire product. The rule-based alternatives are conceptual comparisons, not results from a practical performance test.

### R — Reflection

I learned that AI is used in many everyday systems, often for classification, recognition, prediction, recommendation, and speech processing. I also learned that similar tasks can sometimes be performed using conventional rules, but the results may differ in flexibility and adaptability. When public documentation does not establish how a specific feature works, I should write that there is not enough public evidence to conclude rather than guessing.
---

## Q9. Prediction, Classification, and Generation

### A — Answer

Prediction, classification, and generation describe different kinds of tasks performed by AI systems.

- **Prediction:** Estimates a value or future outcome using available information.
- **Classification:** Assigns an input to a category or label.
- **Generation:** Creates new content, such as text, images, audio, or code.

### Classification of the Eight Examples

| No. | Example | Task category | Explanation |
|---|---|---|---|
| 1 | House-price prediction | Prediction | Estimates a numerical house price using features such as location and size. |
| 2 | Cat image detection | Classification / recognition | Identifies a cat or assigns the image to an appropriate category. |
| 3 | Email writing from an instruction | Generation | Creates new text based on the user's instructions. |
| 4 | Customer churn prediction | Prediction | Estimates whether a customer is likely to stop using a service. If the output is a churn/no-churn label, it can also be treated as classification. |
| 5 | Research paper summarization | Generation | Produces a shorter representation of the original paper. |
| 6 | Fraud transaction detection | Classification | Classifies a transaction as potentially fraudulent or legitimate. |
| 7 | Text-to-image generation | Generation | Creates an image based on a text prompt. |
| 8 | Predicting the next token | Prediction | Estimates a likely next token from the preceding context. |

### Why Next-Token Prediction Matters for LLMs

Many modern LLMs are trained to predict tokens from context. During text generation, the model estimates probabilities for possible next tokens, selects a token according to its decoding method, and repeats the process to produce a sequence.

This process allows an LLM to generate different forms of text, including answers, explanations, summaries, and emails. However, predicting likely text does not guarantee factual correctness. The generated answer may still contain errors or unsupported claims, so important information should be verified.

### E — Evidence

For this question, I will use a reliable technical explanation of language models and next-token prediction. I will also review a source explaining the differences between predictive and generative AI.

Reference for verification:

- Google for Developers, Machine Learning Glossary: https://developers.google.com/machine-learning/glossary

### V — Verification

I checked that each example is assigned according to the main task it performs. House-price estimation and customer churn estimation are prediction tasks; fraud detection and cat recognition involve classification; email writing, paper summarization, and text-to-image creation involve generation. Next-token prediction estimates the next token based on context.

Some categories overlap depending on how a task is formulated. For example, customer churn can be treated as numerical risk prediction or as a binary classification task. I will keep the explanation consistent with the actual output being produced.

### R — Reflection

I learned to distinguish between estimating an outcome, assigning a label, and creating new content. I also learned that next-token prediction is a central mechanism in many modern LLMs, but it does not guarantee that every generated statement is true. Understanding the task type helps me choose appropriate ways to evaluate an AI system.
---

## Q10. Design a Personal AI Verification Protocol

### A — Answer

My personal AI verification protocol is a repeatable process for checking AI-generated information before I rely on it. It helps me identify unsupported claims, incorrect assumptions, calculation errors, and contradictions.

### Seven-Step Verification Protocol

1. **Define the problem.** State exactly what needs to be answered and what a satisfactory answer should contain. This helps catch vague prompts and misunderstandings.

2. **Identify assumptions.** Check the relevant context, conditions, versions, units, and constraints. This helps catch hidden assumptions and incorrect interpretations.

3. **Find authoritative sources.** Look for official documentation, primary references, standards, or other reliable evidence. This helps identify unsupported claims and weak sources.

4. **Verify important claims.** Compare the AI's statements with the evidence and check figures, units, and conditions. This helps catch factual errors, missing details, and contradictions.

5. **Test when appropriate.** Independently recalculate results or use a safe, relevant experiment or simulation. This helps catch errors that may not be obvious from reading the answer.

6. **Decide whether to accept, revise, reject, or leave the answer unresolved.** Accept it when the evidence is sufficient, revise partly correct answers, reject claims contradicted by evidence, and seek further information when the evidence is insufficient. This prevents confidence or fluency from being mistaken for correctness.

7. **Record the evidence and decision.** Keep the prompt, important claims, references, test results, and final conclusion. This makes the decision traceable and helps prevent repeated mistakes.

### Worked Example: Checking a Calculation

**Question:** A notebook costs ₹80. What is the cost of three notebooks before tax?

**AI answer:** ₹240.

I defined the task as calculating the total before tax and assumed that each notebook costs ₹80, with no discount. I verified the result independently:

80 × 3 = ₹240.

A calculator gives the same result. Because the arithmetic agrees with the stated assumptions, I would accept the answer for this simple task and record the calculation as evidence.

If the price, quantity, tax, or discount were uncertain, I would verify those details before accepting the final amount.

### E — Evidence

The worked example uses the stated price and quantity, a direct arithmetic calculation, and an independent calculator check. These are sufficient to verify this simple numerical result under the stated assumptions.

For factual or technical questions, I would use relevant primary references, such as official documentation or manufacturer datasheets. For more consequential decisions, I would use stronger verification and appropriate human review.

### V — Verification

I checked that the seven steps cover problem definition, assumptions, authoritative sources, claim checking, practical testing, a decision to accept or reject or revise, and recording the evidence. In the worked example, the multiplication confirms the total of ₹240 before tax.

The example demonstrates the protocol for a simple calculation; it does not prove that every AI answer is reliable. Different tasks require different kinds and levels of evidence.

### R — Reflection

I learned that AI verification should be a structured process rather than a quick judgment based on how convincing an answer sounds. The level of checking should match the importance and risk of the task. I will use this protocol to check AI-generated information, record evidence, and avoid relying on unsupported claims.




