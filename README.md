# StudyDock AI
Built with **Gemini Canvas** and **ChatGPT**<br><br>
StudyDock AI is an AI-powered study assistant that lets students upload PDF study material, read it inside an integrated viewer, ask questions about it, and generate quizzes from it. It combines document viewing, tutoring, and quiz generation into a single clean interface.

## Features

* **PDF Upload & Viewing**

  * Upload one or more PDF files
  * Built-in PDF viewer with page navigation and zoom controls
  * Switch between uploaded documents easily

* **Tutor Mode**

  * Ask questions based on uploaded study material
  * Receive AI-generated explanations and study help
  * Responses are contextual to the uploaded PDFs

* **Quiz Mode**

  * Generate quizzes from the uploaded material
  * Helps test understanding of a topic from the PDF
  * Separate chat history from Tutor Mode for better organization

* **Student Personalization**

  * Optional **Name** and **Age** fields
  * Can be included in prompts to make responses more student-aware

* **UI Features**

  * Light / dark mode toggle
  * Typing indicator while AI is generating a response
  * Separate Tutor and Quiz chat tabs
  * Warning overlay for portrait mode on smaller screens

## How It Works

1. The user uploads one or more PDF documents.
2. The app extracts text from the PDFs using **PDF.js**.
3. The extracted text is stored and used as context for AI responses.
4. When the user sends a message in **Tutor Mode** or **Quiz Mode**, the app:

   * collects the user’s input,
   * gathers uploaded document text,
   * optionally includes the student’s name and age,
   * sends the prompt to the **Google Gemini API**.
5. The generated response is shown in the chat panel.

## Technologies Used

* **HTML**
* **CSS / Tailwind CSS**
* **JavaScript**
* **PDF.js** – for PDF rendering and text extraction
* **Marked.js** – for rendering Markdown AI responses
* **Google Gemini API** – for tutoring and quiz generation

## Project Structure

StudyDock AI is a front-end web application with:

* a **document upload sidebar**
* a **central PDF viewer**
* an **AI chat sidebar** with Tutor and Quiz modes

The mobile app version is simply the web app loaded inside a web-view container.

## Screens / Main Components

### 1. Document Panel

Used to upload and switch between PDF documents.

### 2. PDF Viewer

Displays the currently selected PDF with:

* page navigation
* zoom in / zoom out
* centered scrollable rendering

### 3. Tutor Chat

Used for asking doubts, explanations, and study help based on uploaded content.

### 4. Quiz Chat

Used for generating quizzes from the uploaded study material.

## Current Limitations

* The AI depends on the quality and clarity of the uploaded PDF text.
* Very large PDFs may need truncation before being sent to the AI.
* Scanned/image-only PDFs may not extract text properly unless OCR is used.
* An internet connection is required for Gemini API-based responses.
* A valid Gemini API key is required to use the AI features.

## Future Improvements

Possible future improvements for StudyDock AI include:

* Multiple-choice quiz generation
* Answer checking and scoring system
* Flashcard generation
* Topic-wise quiz selection
* Better support for scanned PDFs / OCR
* Saving chat history and session data
* Improved mobile app layout and controls

## License

This project is licensed under the **CC BY-SA 4.0** license.

You are free to share and adapt the material as long as proper credit is given and derivative works are distributed under the same license.

## Author

**Roshan Deepu Roy**
