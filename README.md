# Speak full-stack take-home project

## Welcome

Thank you for your interest in Speak! We’re excited to have you in our interview process and hope you have a great experience.

This document outlines the details and guidelines for Speak’s full-stack take-home project.

## Project overview

You’ll build a mini language learning portal: a simple web application where users can browse courses, view lessons, and simulate recording/transcribing speech for a lesson.

- Aim to spend approximately 4–6 hours on this exercise
- Use technologies and frameworks you are most comfortable with
- Persist data via a lightweight database or JSON files
- Feel encouraged to leverage AI tooling to efficiently deliver a solution

## Product requirements

### Pages

- A page presenting a list of available courses
- A page presenting the details and lessons for a single course
- A page presenting the details for a single lesson and a _Record_ button

#### Recording experience

- Simulate sending audio chunks to the backend via WebSocket
- Simulate real-time updates to display transcribed text as it streams in

## Provided assets

- [Courses](/assets/course.json)
- [Audio](/assets/audio-chunks.json)
- [Transcriptions](/assets/audio-transcriptions.json)

## Submission guidelines

- Fork the repository at <https://github.com/usespeakeasy/full-stack-take-home-assessment>, ensuring the fork is private

    ```bash
    gh repo fork usespeakeasy/full-stack-take-home-assessment --clone --visibility private
    ```

- Complete your work in your forked repository
- Add a section to the `README` describing how to run the application locally
- Add the following GitHub users as collaborators to your fork:
  - tc
  - jerrypopsoff
  - ngamolsky
- Send the link to your fork to our recruiter

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

## Onsite presentation

If selected, your take-home project will be a key discussion topic during your onsite interview. Be prepared to present:

- Your architecture and design decisions
- Feature implementation overview
- Bonus features or improvements you’d add with more time
- Challenges faced and how you solved them

Good luck! We look forward to reviewing your work. 🚀
