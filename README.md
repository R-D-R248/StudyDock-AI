# StudyDock AI

StudyDock AI is a web-based study assistant that combines **PDF viewing**, **AI tutoring**, and **AI quiz generation** into a single minimalist workspace.
Users can upload study PDFs, read them inside the built-in viewer, and interact with an AI in two different modes:

* **Tutor Mode** – explains concepts, answers doubts, and simplifies material
* **Quiz Mode** – generates quizzes based on uploaded study content

The project was built as a lightweight student-focused learning tool using **HTML, Tailwind CSS, JavaScript, PDF.js, and the Gemini API**.

---

## Features

### PDF Study Workspace

* Upload and view **multiple PDF files**
* Switch between uploaded documents
* Navigate pages with **Next / Previous**
* Zoom in and out inside the PDF viewer

### AI Tutor Mode

* Ask questions based on uploaded study material
* Receive explanations and simplified answers
* Student name and age can be included in the prompt context

### AI Quiz Mode

* Generate quizzes from the uploaded study material
* Keeps quiz chat separate from tutor chat
* Useful for revision and self-testing

### Chat System

* Separate chat histories for **Tutor** and **Quiz**
* Typing indicator while the AI is generating a response
* Markdown rendering for AI responses

### UI / UX Features

* Minimalist 3-panel layout
* Dark mode toggle
* API key status indicator
* Warning before leaving/reloading the page to reduce accidental loss of progress

---

## Tech Stack

* **HTML**
* **Tailwind CSS**
* **JavaScript**
* **PDF.js**
* **Marked.js**
* **Gemini API**

---

## How It Works

1. Enter your **Gemini API key**
2. Upload one or more **PDF files**
3. Open a document in the built-in viewer
4. Use **Tutor Mode** to ask questions about the material
5. Use **Quiz Mode** to generate quizzes from the same uploaded content

The AI is given the extracted text from uploaded PDFs as context, allowing it to answer questions or create quizzes based on the study material.

---

## Installation / Usage

### Option 1: Run locally

1. Download or clone this repository
2. Open `index.html` in your browser
3. Enter your Gemini API key in the top bar
4. Upload your study PDFs
5. Start using Tutor or Quiz mode

### Option 2: Deploy online

This project can be deployed easily using platforms such as **Vercel** since it is a static frontend project.

---

## Project Structure

```bash
StudyDock-AI/
│
├── index.html        # Main application file
└── README.md         # Project documentation
```

---

## Key Design Choices

### 1. Tutor and Quiz are separated

StudyDock AI keeps **Tutor Mode** and **Quiz Mode** as separate chat systems so that:

* quiz messages do not mix with tutor explanations
* the user gets a cleaner study experience
* different AI tasks stay organized

### 2. PDF + AI in one interface

Instead of switching between a PDF reader and a chatbot, the app keeps:

* documents on the left
* PDF viewer in the center
* AI assistant on the right

This makes studying more seamless and distraction-free.

### 3. Student-friendly context

The app allows a user to enter:

* **Name**
* **Age**

This information can be included in the prompt context so the AI can better tailor its explanations or quizzes.

---

## Limitations

* The project depends on a valid **Gemini API key**
* Large PDFs may take longer to process because text is extracted from all pages
* Chat history is currently session-based and does not persist after closing the tab
* The quality of AI responses depends on the quality of extracted PDF text

---

## Future Improvements

Possible future upgrades for StudyDock AI include:

* Saving chat history using **localStorage** or a database
* Highlighting which PDF section an answer came from
* Generating different quiz types (MCQ, true/false, short answer)
* Better handling for very large PDFs
* Exporting quiz results or study summaries
* More advanced prompt customization for different age groups or subjects

---

## Why I Built This

StudyDock AI was built to make studying from PDFs more interactive.
Instead of passively reading notes or textbooks, students can upload material and immediately:

* ask questions
* get simplified explanations
* revise through quizzes

The goal was to create a lightweight study tool that feels more like a **smart learning dock** than just a PDF reader or a chatbot.

---

## Screenshots

Example:

```md
## Screenshots

### Main Interface
![StudyDock AI Screenshot](screenshot.png)
```

---

## License

This project is currently released for learning / portfolio purposes.
You can add a formal license here later if needed (for example, MIT License).

---

## Author

Made by **Roshan Deepu Roy**<br>
with Gemini Canvas
