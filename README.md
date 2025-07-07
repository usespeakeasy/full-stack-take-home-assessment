# Speak full-stack take-home project

## Welcome

Thank you for your interest in Speak! We’re excited to have you in our interview process and hope you have a great experience.

This document outlines the details and guidelines for Speak’s full-stack take-home project.

---

## Project overview

You’ll build a mini language learning portal: a simple web app where users can browse courses, view lessons, and simulate recording/transcribing speech for a lesson.

- Estimated time: 5–8 hours
- Focus: Clean, well-organized code, solid architecture, and thoughtful trade-offs
- Tech stack: Use any modern frontend (React, Vue, Angular, etc.) and backend (Node.js, Python, etc.) frameworks you’re comfortable with
- Mock data: You may use in-memory data or a lightweight database (e.g., SQLite, MongoDB, or even JSON files)
- Submission: Fork the public repository (see below) and submit your work as a private fork

---

## What you’ll build

### 1. Course list screen

- Display a list of available language courses
- Each course shows:
  - Course title
  - Instructor name
  - Number of lessons
  - Thumbnail image

### 2. Course detail screen

- When a course is selected, show:
  - Course details (title, instructor, description)
  - List of lessons in the course

### 3. Lesson detail and transcription screen

- When a lesson is selected, show:
  - Lesson title and description
  - “Record” button (simulate recording)
  - When “Record” is clicked:
    - Simulate sending audio chunks to the backend via WebSocket
    - Display transcribed text as it streams in (simulate real-time updates)
    - You may use provided mock audio and transcription data, or generate your own

---

## Backend requirements

- REST API to serve:
  - List of courses
  - Course details (including lessons)
  - Lesson details
- WebSocket endpoint to:
  - Accept simulated audio chunks (can be simple JSON messages)
  - Respond with “transcribed” text in streaming fashion (simulate with a delay)
- No need for user authentication (unless you want to add as a bonus)

---

## Frontend requirements

- Course list page
- Course detail page
- Lesson detail/transcription page
- Navigation between pages
- Display streaming transcription as it arrives from the backend

---

## Provided assets

- Sample course and lesson data (JSON)
- Sample audio chunk and transcription data (JSON)
- Sample images/icons (optional)
- The public starter repository to fork

---

## Submission guidelines

- Fork the public repository at:
  [https://github.com/speak-app/language-portal-takehome](https://github.com/speak-app/language-portal-takehome)
- Complete your work in your forked repository.
- Make your fork **private**.
- When you are ready to submit:
  - Add the following GitHub users as collaborators to your private fork:
    - tc
    - jerrypopsoff
    - ngamolsky
  - Send the link to your private fork to our recruiter.
- Include a README describing:
  - Architecture and design decisions
  - How to run the app locally

---

## Judging criteria

- Architecture and code quality
  - Clear separation of concerns (frontend/backend, components, services, etc.)
  - Clean, idiomatic code
- Code readability and documentation
  - Well-organized, easy to follow, and well-documented
- API design
  - RESTful, consistent, and easy to use
- Real-time communication
  - Proper use of WebSocket for streaming transcription
- UI/UX
  - Intuitive, responsive, and visually clear
- Bonus points
  - Unit/integration tests
  - Error handling and edge cases
  - Dark mode support
  - User authentication
  - Dockerization for easy setup

---

## Example data

courses.json

```json
[
  {
    "id": "course1",
    "title": "Beginner Korean",
    "instructor": "Jane Kim",
    "thumbnail": "/images/korean.png",
    "description": "Start speaking Korean from day one!",
    "lessons": [
      { "id": "lesson1", "title": "Greetings", "description": "Learn how to say hello." },
      { "id": "lesson2", "title": "Numbers", "description": "Counting in Korean." }
    ]
  }
]
```

transcription-chunks.json

```json
[
  { "chunk": "audio1", "text": "안녕하세요", "delayMs": 500 },
  { "chunk": "audio2", "text": "Hello", "delayMs": 700 },
  { "chunk": "audio3", "text": "How are you?", "delayMs": 600 }
]
```

---

## Onsite presentation

If selected, your take-home project will be a key discussion topic during your onsite interview. Be prepared to present:

- Your architecture and design decisions
- Feature implementation overview
- Bonus features or improvements you’d add with more time
- Challenges faced and how you solved them

---

Good luck! We look forward to reviewing your work. 🚀
