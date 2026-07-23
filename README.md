# n8n-post-meeting-automation
🎙️ Post-Meeting Automation Workflow (n8n + OpenAI + Telegram + Gmail)
A comprehensive n8n workflow that automates the processing of business meeting video and audio recordings. The system fetches files from Google Drive, handles transcription and conversion, and provides an interactive Telegram menu featuring human-in-the-loop automation.

🚀 Key Features

•	Google Drive & CloudConvert Integration: Automatically detects new recordings in a selected folder and converts video files into optimal audio format (.mp3).

•	AI Audio Transcribe: Processes speech-to-text using the OpenAI Whisper model.

•	Interactive Telegram Menu: Human-in-the-loop decision-making for processing paths:

•	Quick Notes: Summary of key decisions sent to Telegram and email.

•	Action Items: Task list extraction featuring an approval system prior to team dispatch.

•	Follow-Up Presentation (PDF): Automatic HTML/CSS layout generation converted into a professional PDF file.

•	HTML-to-PDF Engine: Dynamic business slide design in HTML/CSS integrated with structured JSON data from OpenAI.

•	Interactive Email Dispatch: Collects client email addresses via Telegram and dispatches a dedicated HTML email with the attached PDF.

🛠️ Technologies & Nodes

•	Automation: n8n (v1.x)

•	AI Models: OpenAI API (GPT-4o-mini, Audio Transcription)

•	Messaging & HITL: Telegram Bot API (sendAndWait, sendDocument)

•	Document Generation: Custom JavaScript Code (HTML/CSS layout) + HTML-to-PDF engine

•	Storage & Mail: Google Drive API, CloudConvert API, Gmail API

📥 Installation Guide

	1.	Download the workflow file from the repository (workflow.json).
	
	2.	Open your n8n environment, select Import from File, and paste the content.
	
	3.	Configure the required credentials:

•	OpenAI API Key

•	Telegram Bot Credentials

•	Google Drive & Gmail OAuth2

•	CloudConvert API Key

•	HTML2PDF API Key

	4.	Activate the workflow!
