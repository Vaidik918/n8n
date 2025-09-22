Vaidik's n8n Automation Portfolio

This repository contains a collection of advanced workflow automation projects built with n8n (https://n8n.io/). These projects demonstrate the ability to integrate various APIs, handle complex logic, and build intelligent, real-world solutions that solve tangible business problems.

Projects

1.  WhatsApp Turf Booking Bot: A fully conversational AI bot that automates the entire process of booking a sports turf via WhatsApp.
2.  Email to WhatsApp Notification System: A real-time monitoring workflow that sends instant WhatsApp alerts for important emails.

Project 1: WhatsApp Turf Booking Bot

This project transforms the tedious, manual process of phone-call-based turf booking into a seamless, automated experience managed by a smart assistant on WhatsApp.

Key Features

- Conversational AI: Powered by Google Gemini to understand natural language requests (e.g., "kal shaam 5 baje ka slot hai?").
- Multi-Turn Conversation Memory: Remembers the context of the conversation using Google Sheets as a database. If a user provides partial information, the bot intelligently asks for the missing details.
- Real-time Availability Check: Integrates directly with Google Calendar to check for booked slots in real-time.
- Intelligent Slot Suggestions: If a requested slot is unavailable, the bot analyzes the calendar and suggests alternative available time slots.
- Payment Integration: Automatically generates Razorpay payment links to collect advance booking fees.
- End-to-End Automation: Handles the entire flow from initial enquiry to final confirmation, including notifying the turf owner.

Tech Stack & n8n Nodes Used

- Core Engine: n8n (Self-Hosted via Docker)
- Messaging Interface: Twilio (WhatsApp API)
- AI & Language Model: Google Gemini
- Conversation Memory: Google Sheets
- Scheduling: Google Calendar
- Payments: Razorpay (via HTTP Request Node)
- Core Logic: Webhook, Code (JavaScript), IF, and Merge nodes.


Project 2: Email to WhatsApp Notification System

This workflow acts as a personal, high-priority alert system. It actively monitors an email inbox and sends an immediate WhatsApp notification when an email matching specific criteria arrives.

Key Features

- Real-time Monitoring: Uses the IMAP protocol to instantly trigger the workflow upon receiving a new email.
- Smart Keyword Filtering: The workflow is configured to only process emails that contain a specific keyword (e.g., your name) in the subject line.
- Instant WhatsApp Alerts: Delivers a clean, formatted notification directly to your phone via the Twilio WhatsApp API.
- Dynamic Content: The notification message includes key details from the email, such as the sender and the subject line.

Tech Stack & n8n Nodes Used

- Core Engine: n8n
- Data Source: IMAP Email Node
- Notification Channel: Twilio Node
- Logic: IF Node


Business Compliance Information (for API Verification)

Terms of Service
This is a portfolio project for demonstration and educational purposes. Any bookings or transactions generated via this system are not final and are for testing only.

Privacy Policy
We do not store any personal user data beyond the temporary information (phone number, requested time) required to process a booking request during a session. All session data is cleared after a booking is finalized or canceled.

Contact Us
- Name: Vaidik Mane
- Email: vaidik0918@gmail.com
