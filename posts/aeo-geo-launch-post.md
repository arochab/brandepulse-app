# Post AEO/GEO — Launch posts

> Adam : à adapter à ta voix avant de poster.

---

## Version Reddit (r/SEO)

**Title:** I mapped share of voice across SERP and AI for 5 brands in one niche. Here's what the data says.

**Body:**

I've been working on the gap between traditional search rankings and what AI engines actually recommend when someone asks a buyer intent question like "best X for Y." Two very different signals, and the delta between them is where the real GEO/AEO opportunity sits.

I built a tool to measure both at once. You type one brand name, it identifies your competitive set and buyer intent queries automatically, then runs them against live Google via Bright Data and checks which brands an AI engine would recommend for the same queries. You get a dual heatmap showing SERP position vs AI mention order, side by side.

What I found surprised me. Brands with strong content marketing get boosted in AI recommendations even when they rank 4th or 5th on SERP. And the reverse happens too: some brands own position 1 on Google but get zero AI mentions. That gap is invisible if you only track rankings.

Example: I ran Notion. It sits at #3 for "best project management tool" on SERP, but AI engines rank it #1. Asana takes #2 on SERP and #2 on AI. Coda is at #6 on SERP but jumps to #3 in AI recommendations. The gap between those two heatmaps tells you exactly where your GEO strategy should focus.

The tool is live at brandpulse-app.onrender.com. Pro plans for ongoing monitoring are launching soon. Curious what signals beyond SERP rank and AI mentions you think are worth tracking for GEO.

---

## Version Reddit (r/SaaS)

**Title:** I built a competitive visibility tool that maps SERP and AI search side by side. Here's the architecture.

**Body:**

I wanted to know whether my product shows up when someone searches "best [tool] for [use case]" and I wanted to compare that to what AI engines recommend for the same question. No existing tool maps both signals.

So I built one. You type a brand name and the system does four things: identifies your competitors and buyer intent queries automatically, runs them against live Google, checks which brands an AI assistant would recommend for the same queries, and renders both as a dual heatmap. Green cells for SERP ranks, purple cells for AI mention order.

The interesting insight is that those two heatmaps rarely match. Some brands dominate SERP but are invisible to AI. Others have weak search rankings but show up first in AI recommendations. That delta is the signal.

Stack: Python/Flask backend, Claude Haiku for competitive intelligence inference and AI visibility simulation (two API calls per analysis), Bright Data for live SERP, vanilla JS frontend. The AI check is a single structured prompt where Claude answers buyer queries as an AI assistant would, which gives you a proxy for AI engine mention order without paying for 5 different API integrations.

The tool is live at brandpulse-app.onrender.com. Pro plans with ongoing monitoring and alerts are coming soon. I can go deeper on the AI visibility methodology or the architecture if anyone's interested.
