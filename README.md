# Executive Email AI Agent

## Overview
This AI-powered executive email assistant automates email classification and response drafting using **LangGraph, Gemini, and the Gmail API**. The agent is designed to streamline email management by categorizing emails and assisting users in crafting responses efficiently while keeping a **human-in-the-loop** for validation and refinement.

## Features
- **Email Fetching:** Retrieves unread emails from the inbox.
- **Classification:** Categorizes emails into:
  - `Respond`
  - `Don't Respond`
  - `Notify`
  - `Doubtful` (asks for user input before classification)
- **Human-in-the-Loop:**
  - If classified as `Respond`, prompts the user for relevant facts to draft an appropriate reply.
  - Iteratively refines the draft based on user feedback until satisfaction is achieved.
- **Memory Integration:** Maintains context for better decision-making in classification and drafting.

## Tech Stack
- **LangGraph** – Manages workflow logic and state transitions.
- **Gemini API** – Generates and refines email responses.
- **Gmail API** – Fetches emails and drafts responses.

## How It Works
1. Fetches unread emails from the inbox.
2. Classifies emails using an AI model.
3. If unsure, asks the user to manually classify the email.
4. For `Respond` emails:
   - Asks the user for key facts.
   - Drafts an email using AI.
   - Iteratively refines the draft based on user feedback.
5. Finalizes and saves the draft email for the user.


## Contributing
Feel free to open issues or contribute via pull requests!

