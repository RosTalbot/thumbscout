# 🧠 ThumbScout 
*ThumbScout* is an AI-powered research agent that assists content teams in identifying visual trends across top-performing YouTube thumbnails. It helps creators make data-driven packaging decisions by scraping competitive video results, analyzing visual styles, and surfacing repeatable trends or opportunities to stand out.

This tool is designed for solo creators, marketing teams, and content strategists who want to improve YouTube performance without wasting hours manually researching thumbnails.

🛑 License: TBD — Waiting on project partner feedback before open-sourcing under MIT or other license.

⸻

## 🚀 Core Features
- 🔍 Topic-Based Research
Enter a video topic and instantly get top-performing YouTube thumbnails + metadata.
- 🧠 Visual Trend Analysis
Uses GPT-4 Vision (or Claude 3 Opus) to detect patterns in thumbnails (e.g. colors, faces, text styles).
- 💡 Smart Suggestions
Recommends either trend-matching or disruptive thumbnail concepts based on market data.
- 📊 Packaging Insights
Optionally integrates A/B test learnings to refine future thumbnail prompts.

⸻

## 📦 MVP Goals (Bootcamp Build)
- Accept static or scraped video list for a YouTube topic
- Return a formatted visual + metadata grid (title, views, publish date, etc.)
- Output a written trend summary and design direction suggestions
- Optional: Export to Notion or display HTML dashboard

⸻

## 🔧 Tech Stack

- Language Model:	GPT-4 (Vision) or Claude 3 Opus
- Data Source:	SERP API (YouTube search via Google)
- Environment:	n8n or Replit (Node.js)
- _Optional Storage:	Notion DB, Google Drive_


⸻

## 🧠 Agent Context-Awareness

- Understands the creator’s brand goals (future)
- Tracks topic → trends → output for feedback loops
- Adapts tone and suggestions based on creator persona (future upgrade)

⸻

## 💼 Real-World Use Cases
- YouTube agencies performing competitive research
- Creators planning thumbnails that break through visual noise
- Strategists testing thumbnails and refining based on actual viewer behavior

⸻

## 🧪 Evaluation & Limitations
<details><summary>Click to expand</summary>

### ✅ Project Evaluation: ThumbScout MVP (First Run)

- Project Name: ThumbScout
- Creator: Ros Talbot
- Date: July 31, 2025
- Version: MVP v0.1
- Duration: ~2 hours

### 🔧 Project Summary

ThumbScout is an AI-powered thumbnail research assistant designed to analyze YouTube video titles for hook strength, emotional appeal, and formatting techniques. The current MVP scrapes real titles from YouTube-related content via SerpAPI, evaluates them using GPT (3.5 or 4), formats the results into a CSV, and sends them as an email report to the user.


### 🎯 What’s Working (MVP Successes)
- **Automated Data Pipeline**
  - Live search → OpenAI analysis → file conversion → email delivery.
  - End-to-end automation successfully tested with real input/output.
- **Multi-tool Orchestration**
  - Seamless integration of n8n, SerpAPI, GPT, file conversion, and native email sending (no OAuth required).
  - Used n8n’s file handling nodes and logic chains with confidence.
- **Scoping & Execution**
  - Load reduced from 20 to 5 items mid-run to manage execution time and cost.
  - Both Turbo and GPT-4 output formatting.
- Human-Centered Output
  - CSV file was clear, readable, and attached automatically in a styled email.
  - Subject line dynamically included the date and was branded as a “ThumbScout Report.”


### 🛠 Opportunities for Improvement
- Limited Search Input
- → Current SerpAPI query is short and broad. Niche-specific strings would yield more dialed-in, relevant titles for better insights.
- Manual Execution Bottlenecks
- → Workflow currently requires manual step-by-step execution in n8n. Needs triggers or chaining for a true one-click (or scheduled) experience.
- Output Structure & Context
- → GPT responses are dumped into a single message.content field. Needs parsing into structured fields (e.g., Hook Type, Format Style, Emotional Appeal).
- → Source attribution is missing—no original URLs or video titles are included for traceability.
- Redundant Data Columns
- → Output includes unnecessary GPT metadata like message.role, refusal, etc., which could be stripped out in a clean-up step.


### 💡 Next Steps
- Add structured parsing to GPT outputs (Markdown, HTML, or JSON)
- Strip extraneous export columns for better CSV readability
- Include video title, channel name, or link from SerpAPI in final output
- Automate full run from query to delivery with a single trigger
- Explore multi-keyword batch prompts for greater context efficiency

### 🏅 Overall Evaluation

### ✅ MVP Criteria Met
- 🌱 Functional, Real-World Utility Delivered
_🚀 Strong Candidate for Iterative Expansion (v0.2+)

</details>

⸻


## 📈 Future Directions
- 🔁 A/B test result feedback loop
- 🤖 Persona-based suggestions (e.g. bold marketer vs clean strategist)
- 🧰 Prompt bank generator for thumbnail designers
- 📸 Image grid export or embedded dashboard

⸻

💬 Questions? Ideas?

DM @RosTalbot or fork the repo and try it yourself!
