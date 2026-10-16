# My Rule-Based Chatbot

For this CodSoft task, I made a small browser chatbot called Milo. You can type a message or use the suggestion buttons, and Milo looks for familiar words and phrases before choosing a response.

I gave Milo its own dark indigo and violet chat-app look, with coral accents, so this project feels different from my Tic-Tac-Toe game.

## Try it out

1. Open `index.html` in a modern web browser.
2. Type a message in the box, or choose one of the example prompts.
3. Press Enter or select the send arrow.
4. Select **Clear chat** to start again.

Milo understands greetings, questions about its name, the time and date, jokes, study tips, thanks, and goodbyes. If it does not recognize a message, it gives a friendly prompt with examples of things to ask.

## How the response rules work

Before checking a message, the JavaScript code makes it lowercase, trims extra spaces, and removes most punctuation. Then `getResponse()` checks the message against regular-expression patterns in order. The first matching rule supplies the reply. A final fallback response handles messages that do not match any rule.

For example, a message containing “hello”, “hi”, or “hey” matches the greeting rule. A message asking “what time is it?” matches the time rule, which gets the current time from the browser. The chatbot does not learn from messages or use an online AI service; its replies come from the rules in the code.

## What I learned

This project gave me practice with basic text normalization, pattern matching, and organizing rules into a conversation flow. I also learned how to show messages in a browser interface and keep the interaction simple to use.

## Project files

- `index.html` contains the chat interface, styling, and response logic.
- `README.md` explains how to run the chatbot and how its rules work.
- `Project_Report.pdf` is a short report for my project submission.
