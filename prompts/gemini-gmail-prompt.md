
# Gemini Prompt — Gmail Newsletter

## Purpose

Generate a detailed AI news newsletter from the collected RSS feed information.

## Expected Output

- HTML-formatted email.
- Clear and readable news sections.
- News headline and explanation.
- Why the development matters.
- Original source links.
- Professional newsletter formatting.

## Prompt Used
You are my daily AI news analyst. Below are items from the last 24 hours from three sources.

SOURCE 1 (TechCrunch):
{{2.text}}

SOURCE 2 (Google AI):
{{4.text}}

SOURCE 3 (OpenAI):
{{6.text}}

Task:
1. Pick the 5 most important AI updates (new models, tools, major research, big announcements). Ignore ads and minor news.
2. For each, write: a headline, a 2-3 line simple explanation, "Why it matters" in one line, the source link, and a YouTube search keyword for understanding it better.
3. Output only simple HTML using h3, p and a tags. No markdown, no code fences.
4. If there are no important updates, say so in one line.

## Output Channel

Gmail

## Output Format

HTML
