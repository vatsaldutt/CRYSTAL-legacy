# CRYSTAL0 (Legacy)
Version from May 4, 2021\
Original Repo: https://github.com/vatdut8994/All-code/tree/main/python/raspi%20code \
Superceding version: https://github.com/vatsaldutt/CRYSTAL-R0.git

---

CRYSTAL0 is the original, experimental version of CRYSTAL. This version was built primarily as a learning project, following a YouTube tutorial on basic machine learning chatbots, and then extended well beyond the tutorial’s scope.
At its core, CRYSTAL0 is a rule-based / ML-assisted chatbot capable of classifying simple prompt categories such as greetings, farewells, and basic conversational phrases (e.g., “hello”, “bye”, “how are you?”). Once a category was detected, the bot would respond using a randomly selected reply from a hard-coded response list for that category. Despite its simplicity, it could generalize slightly across variations in phrasing through basic word tokenization.

![Overview](assets/UI.png)

### Architecture (Legacy / Monolithic Design)

CRYSTAL0 was implemented as a single, monolithic Python script combining:

* UI logic (Tkinter)
* Speech recognition and synthesis
* Translation pipeline
* Intent classification (Keras + NLTK)
* Action execution (web, email, system tasks)

While this structure was not modular or scalable, it enabled rapid experimentation and served as a critical learning phase before later architectural refactors in subsequent CRYSTAL versions.

### Key Contributions Beyond the Tutorial

While the ML logic followed a tutorial, several major features were independently designed and implemented:

* **Multilingual Support via Google Translator**
  CRYSTAL0 could understand and respond in virtually any language, translating user input into English for processing and translating responses back into the user’s language. This significantly expanded its usability beyond English-only chatbots.

* **Custom Graphical User Interface (Tkinter)**
  A fully custom GUI was built using **Tkinter**, providing a visual chat interface rather than a terminal-based experience. This UI laid the groundwork for later CRYSTAL interfaces.

### Features

* ML-based intent classification using Keras and bag-of-words tokenization
* Rule-based response selection with randomized replies
* Voice input using Google Speech Recognition
* Text-to-speech output via gTTS
* Full multilingual support using Google Translate
* Wake-word detection
* Website launching via voice or text commands
* Wikipedia search with automatic fallback to Google search
* Email sending via SMTP (predefined contacts)
* Time and date awareness
* Custom full-screen Tkinter GUI

### Intent-Based Actions (Early Assistant Capabilities)

Beyond conversational replies, CRYSTAL0 supported several action-oriented intents.
These intents triggered direct system or web actions rather than static responses.

Examples include:

* **Website Launching**
  Voice or text commands such as “open YouTube” or “open Google” triggered browser launches using Python’s `webbrowser` module.

* **Wikipedia Search**
  Informational queries were routed to Wikipedia, summarized, and read aloud. If a page was unavailable or ambiguous, CRYSTAL0 automatically fell back to a Google search.

* **Email Sending**
  Predefined email intents allowed CRYSTAL0 to send emails via SMTP using voice input for message content.

These capabilities were implemented through intent classification combined with hard-coded execution logic, rather than dynamic reasoning or planning.


### What It Was (and Wasn’t)

CRYSTAL0 was not a conversationally intelligent system, nor did it maintain memory, context, or reasoning capabilities.
Its “intelligence” was limited to intent classification and hard-coded behaviors.

However, it was an early voice-enabled personal assistant prototype that combined machine learning, UI design, speech I/O, translation, and action execution in a single system.

This version is preserved just for history, showing the evolution from a simple rule-based chatbot into more advanced CRYSTAL iterations.
