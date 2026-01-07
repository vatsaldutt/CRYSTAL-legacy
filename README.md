# CRYSTAL0 (Legacy)
Version from May 4, 2021\
Original Repo: https://github.com/vatdut8994/All-code/tree/main/python/raspi%20code \
Superceding version: https://github.com/vatsaldutt/CRYSTAL-Mark-I.git

---

CRYSTAL0 is the original, experimental version of CRYSTAL. This version was built primarily as a learning project, following a YouTube tutorial on basic machine learning chatbots, and then extended well beyond the tutorial’s scope.
At its core, CRYSTAL0 is a rule-based / ML-assisted chatbot capable of classifying simple prompt categories such as greetings, farewells, and basic conversational phrases (e.g., “hello”, “bye”, “how are you?”). Once a category was detected, the bot would respond using a randomly selected reply from a hard-coded response list for that category. Despite its simplicity, it could generalize slightly across variations in phrasing through basic word tokenization.

![Overview](assets/UI.png)

### Key Contributions Beyond the Tutorial

While the ML logic followed a tutorial, several major features were independently designed and implemented:

* **Multilingual Support via Google Translator**
  CRYSTAL0 could understand and respond in virtually any language, translating user input into English for processing and translating responses back into the user’s language. This significantly expanded its usability beyond English-only chatbots.

* **Custom Graphical User Interface (Tkinter)**
  A fully custom GUI was built using **Tkinter**, providing a visual chat interface rather than a terminal-based experience. This UI laid the groundwork for later CRYSTAL interfaces.

### Features

* Basic machine learning–based intent classification
* Simple word tokenization for prompt generalization
* Rule-based response selection
* Multilingual input/output using Google Translate
* Early speech recognition experiments
* Custom Tkinter-based graphical interface

### What It Was (and Wasn’t)

CRYSTAL0 was not a true conversational AI, nor was it context-aware or generative. It was a proof-of-concept and learning milestone, the foundation that made later versions possible. Think of it as the “hello world” phase of CRYSTAL, but with ambition.

This version is preserved just for history, showing the evolution from a simple rule-based chatbot into more advanced CRYSTAL iterations.
