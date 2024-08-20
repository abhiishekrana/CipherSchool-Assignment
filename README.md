	Full-Stack Developer Assignment
		Introduction
	This project is developed as part of a Full-Stack Developer assignment. The task was to create a web-based Test Environment Platform where students can take multiple-choice questions 		(MCQ) tests. The platform includes user authentication, test administration, and automated evaluation and result delivery via email.

	Table of Contents
	Project Overview
	Platform Requirements
	Technical Stack
	Installation and Setup
	Environment Variables
	Features
	Evaluation and Scoring
	Email Template
	Screenshots
	Future Enhancements

	 Project Overview
		The platform is designed to allow students to log in, take an MCQ test under a secure environment (camera and microphone permissions), and submit their answers. After 			submission, the platform automatically evaluates the test and sends the score to the user via email.

	Platform Requirements
	User Authentication
	Implemented a secure login system using email and password.
	Users must be authenticated before accessing any tests.
	Test Environment
	After login, users are prompted to grant camera and microphone permissions.
	Displays a preview of the camera feed; shows error messages if permissions are denied.
	MCQ Test Interface
	Displays questions with multiple choices, allowing users to select and change their answers.
	Users can navigate freely between questions.
	Includes a camera window in the test interface to ensure a secure test environment.
	Test Submission
	Upon completion, users can submit their test and are redirected to a "Finish Test" page.
	A cron job runs hourly to evaluate the tests and store the results.
	Evaluation and Score Delivery
	The cron job calculates the user's score based on their answers.
	The score is sent to the user’s email using a predefined template.
	Technical Stack
	Frontend: React.js
	Backend: Node.js with Express
	Database: MongoDB
	Authentication: JWT or session-based authentication
	Cron Jobs: node-cron or similar library
	Email Service: Nodemailer, Mailersend, or equivalent
