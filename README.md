# MediAssist
MediAssist is a conversational clinic assistance system. A patient sends a normal Telegram message in English, Hindi or Hinglish. 
The system identifies the patient’s request, asks only the information needed for the next step, and stores confirmed clinic actions in MongoDB. It supports appointment booking, rescheduling, cancellation, complaints and general clinic-related help.
The design separates interpretation from authorization. Groq interprets free-text messages into a strict JSON structure, while deterministic n8n Code nodes validate menu choices, ownership, profile details, slot availability and explicit confirmation before any database change is made.
The first implementation is an academic project prototype with a reusable backend. The visual clinic dashboard is planned as the next interface layer and is represented in the current export by protected dashboard API endpoints.
