# Maximus AI — Portfolio Prototype (Improved)

A responsive, single-page front-end prototype for an AI-powered workplace productivity assistant.

## Features
- Smart Email Generator with editable draft output and copy action.
- Meeting Notes Summarizer with decisions, action items, and risks.
- Task Planner with priorities, completion tracking, and a basic daily schedule.
- Research Assistant that creates a brief from user-supplied source text.
- Browser-local task persistence using `localStorage`.
- Responsible AI notice and clear demo-mode labeling.
- No build tools or third-party dependencies required.

## Run locally
1. Extract the ZIP file.
2. Open `index.html` in a modern browser (Chrome recommended).
3. Add a task or mark one complete, then refresh the page to test task persistence.
4. Generate any output and click inside the result area to edit it; use the Copy button when ready.

## Important limitations
This is a front-end demo. It does **not** connect to OpenAI or Gemini. Outputs are generated using templates and text-matching rules, not a live AI model. It does not browse the web, send email, or connect to a real calendar. Dashboard time-saved values are illustrative estimates, not measured results.

Tasks are stored only in the current browser profile on the current device. Clearing browser storage, using another browser/profile, or browser privacy settings may remove or prevent persistence. Do not store confidential or sensitive business information in this prototype.

## Suggested next step: connect a live model
Add a server-side endpoint (for example, a Supabase Edge Function) that accepts a validated tool name and user input, constructs a structured prompt, calls your chosen AI provider, and returns the result. Store provider keys only as server-side secrets. Never place API keys in `index.html` or other public frontend files.

## Portfolio description
Maximus AI is a responsive productivity-assistant prototype exploring four professional use cases: email drafting, meeting-note summarization, task planning, and source-grounded research briefs. It demonstrates prompt design, editable outputs, browser-local task persistence, human-in-the-loop review, privacy awareness, transparent demo labeling, and a plan for measuring productivity against a manual baseline.


**Theme:** The interface uses a royal-blue page background (`#4169E1`) with white workspace cards for contrast.
