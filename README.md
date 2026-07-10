# Enterprise IT Incident Routing Automation

## Project Description
An automated, AI-powered Level-1 (L1) DevOps Triage Pipeline built using **IBM watsonx Assistant**. This project was developed as a core deliverable for the **4-week IBM SkillsBuild Internship** program. The assistant leverages Natural Language Understanding (NLU) to instantly classify, analyze, and route critical system production errors to specialized engineering rotation teams without requiring manual human triage.

## Author
* **Vibhuti Sharma** (IBM SkillsBuild Intern)

## Core Features Implemented
* **Natural Language Processing:** Recognizes incident trigger phrases like "System Error" to initialize automated triage.
* **Multi-Branch Conditional Routing:** Mapped separate logic paths for critical production server responses:
  * **500 Internal Server Error:** Dispatches database extraction priority logs to Backend DevOps teams.
  * **401 Unauthorized Access:** Flags API gateway handshake failures and alerts the Security Operations Center (SOC).
  * **404 Not Found:** Isolates unmapped resource links and routes lower-priority triage tickets to Frontend Engineering.
* **Session Optimization:** Uses explicit execution termination parameters (`End the action`) to prevent response bleeding between test states.

## Tech Stack
* IBM watsonx Assistant (Conversational AI Platform)
* Dialog Management & Intent Disambiguation Architecture

## How to Import & Test
1. Create a free account on IBM Cloud and launch watsonx Assistant.
2. Go to your Assistant settings, navigate to **Download/Upload**, and choose the **Upload** tab.
3. Upload the project zip/json file from this repository to instantly clone the logic.
4. Open the live preview panel and type "System Error" to run runtime tests.
