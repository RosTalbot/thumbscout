# 🧠 ThumbScout
*ThumbScout* is an AI-powered research agent (in development) designed to analyze top-performing YouTube thumbnails for visual trends, emotional hooks, and formatting strategies. The system aims to help creators make smarter packaging decisions based on real-world viewer behavior.

While this repository is still in early planning stages, it serves as the future home for a complete, end-to-end thumbnail research and analysis tool.

🔧 *Note: The prototype MVP for title/hook analysis has been moved to a standalone project: [TrendScout](https://github.com/RosTalbot/trendscout).* This served as a lightweight POC for text-only trend analysis and now lives as **Vibe Agent 01: TrendScout**.

⸻

## 🔭 Future Scope (ThumbScout v1+)

### 🔍 Inputs
- YouTube video topic or niche
- Optional: competitor channels or specific video URLs

### 🧠 Agent Capabilities
- Scrape YouTube/Google search results via SerpAPI
- Analyze thumbnails using GPT-4 Vision
- Detect visual styles, emotional cues, text placement, color schemes
- Identify patterns (e.g. faces, objects, emojis, font types)
- Score each image on clickability or trend alignment

### 📊 Output Formats
- Markdown trend summary (copy/paste or export)
- Image grid of top thumbnails
- CSV or Notion export with visual descriptors
- Optional: A/B test results overlay for feedback loop

⸻

## 🛠️ Tech Stack
- **LLMs**: GPT-4 (Vision) or Claude 3 Opus
- **Scraping**: SerpAPI
- **Orchestration**: n8n (Cloud or Self-Hosted)
- **Optional Storage**: Notion DB, Google Drive, Firebase

⸻

## 🚧 Status
ThumbScout is currently in design and prototyping. You can preview early trend analysis logic inside [TrendScout](https://github.com/RosTalbot/trendscout), which handles video title analysis and GPT-generated trend summaries. The visual analysis layer is planned for v1.1+.

⸻

💬 Questions? Ideas?
DM [@RosTalbot](https://github.com/RosTalbot) or fork the repo to contribute.
