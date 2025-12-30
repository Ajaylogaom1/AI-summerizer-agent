# AI-summerizer-agent

📁 Google Drive → AI Processing → Google Sheets (n8n Workflow)

This repository contains an automated workflow built with n8n that detects new files uploaded to Google Drive, extracts CSV data, processes it using Google Gemini AI, and appends the results into a Google Sheet.

#🚀 Workflow Functionality

Watches a Google Drive folder for newly added files

Automatically downloads the uploaded file

Extracts CSV content into structured rows

Sends data to an AI Agent powered by Google Gemini for processing

Appends processed results into a Google Sheet

#🧩 Workflow Steps Overview

1️⃣ Google Drive Trigger – Detects a new file added in Drive
2️⃣ Download File – Downloads the CSV file content
3️⃣ Extract From File – Parses CSV into row-wise JSON
4️⃣ AI Agent (Gemini Chat Model) – AI processes & enhances each row
5️⃣ Append Row in Sheet – Inserts the processed result into Google Sheets

#🛠️ Prerequisites

To run this workflow, you need:

An n8n account (self-host or cloud)

Google Drive API credentials

Google Sheets API credentials

Google Gemini API key

🔧 Setup Instructions

1️⃣ Import this workflow JSON into n8n
2️⃣ Add your Google Drive, Sheets and Gemini credentials
3️⃣ Set the Google Drive folder ID in the trigger node
4️⃣ Set the target Google Sheet ID in the append-row node
5️⃣ Upload a CSV file to test – the workflow will run automatically

#🧠 AI Output

Gemini processes each row based on prompts inside the AI Agent node.
You can modify the instructions inside the node to customize the result (e.g., summarization, formatting, extraction).
