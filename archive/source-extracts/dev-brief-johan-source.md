# Source extract — The Gift Whisperer – Dev Brief - till Johan.docx

> **Archive status:** historical source extract.  
> This file preserves machine-extracted text from the original project artifact. Formatting, visual design, embedded media, speaker notes, and layout may not be fully represented.  
> Do not silently normalize historical naming. See [HISTORY.md](../../HISTORY.md) and [SOURCE_INDEX.md](../../SOURCE_INDEX.md).

---

The Gift Whisperer – Dev Brief





Directive: Brand and Operational Naming

METOYO is the public-facing brand, condition, and ritual space within which this system exists.

The Gift Whisperer is the internal operational engine that runs the system inside METOYO. It functions as the working logic, prompt architecture, and execution intelligence that enables memory-driven gifting and reflective gesture.

This distinction is intentional. The operational logic, processes, routines, and system architecture described in these documents remain unchanged. Only the external naming and narrative framing evolve.

“The Gift Whisperer” should be understood as a working dwarf: an internal actor that performs the work without claiming the stage. Over time, this internal actor may evolve into a dedicated AI agent or equivalent system component. This evolution does not alter the identity, purpose, or framing of METOYO.

All references to system behavior, prompts, personas, and operational mechanics continue to apply as written. METOYO names the space and condition; The Gift Whisperer runs the place.








To: [Friend’s name]
From: Linus Fast / Form & Flöde
Subject: Frontend Setup & Soft Build Support for Ritual Prompt System



👁️ Project Overview

The Gift Whisperer is a poetic AI prompt system designed to help people give more emotionally resonant gifts by remembering small, meaningful moments about the people in their lives.
It’s not an app, not a marketplace, and it doesn’t collect data.

Instead, it’s a ritual interface: users input a few memory-based keywords (like “mint tea, rain, his jacket”), choose a persona (like “The Friend” or “The Mentor”), and are taken to a prompt in ChatGPT that suggests:

A fitting gift idea

Where to get it

How to present it with emotional weight

The goal is to make people feel confident, present, and emotionally aware — especially in situations where gifting feels rushed or stressful.



🔧 What I Need Help With (Now)

A simple Carrd site (or similar frontend) that does this:

Presents 7–10 persona cards the user can scroll through (e.g. The Friend, The Colleague, The Romantic Other)

Each card links to a pre-written ChatGPT prompt with 3–5 blank fields for user keywords (we’ll pre-structure these links)

A soft intro and outro page with a bit of poetic storytelling

Optional: a way to track which links are clicked (Bitly, UTM, or GA4 with Tag Manager)

Optional: form embed (Tally or Typeform) to collect anonymous stories from users after giving a gift

I have:

Full content (text, tone, structure)

A tone/UX guide

All prompt links ready

Reference decks and system descriptions if needed



🧱 Technical Stack (Chosen for Simplicity)

Carrd.co: Mobile-first, no login, low code

ChatGPT Prompt Links: Custom URL strings to pre-fill GPT prompts

Bitly or UTM: For link tracking

Google Analytics 4 + Tag Manager: For light interaction data

Tally.so or Typeform: For collecting “gift reflection” stories

Zapier (optional): For connecting form data to a sheet or GA

If you know a better stack for this simplicity + poetic flow, open to that too.



⚙️ Milestone Tasks (what could be built together)

Phase 1 — MVP

Carrd site with 1 page per persona → links to GPT prompts

Soft landing and closing page (intro/outro storytelling)

Link tracking + UTM setup

Phase 2 — Refined UX

Icons + colors for each persona

Prompt selector logic (choose persona + enter 3 keywords → click)

Story submission form (Tally embed)

Light dashboard with Looker Studio

Phase 3 — Artifact Output

Printable zine version (optional layout support)

Prompt card generator (HTML export or Notion integration)



🔐 Ethos & Legal

This project is:

100% non-commercial (Creative Commons BY-NC-SA 4.0)

Hosted under my company Form & Flöde

GDPR-compliant by design: no tracking, no storage, forget-by-default

You’ll be covered by a short Contributor Agreement I already drafted (friendly, open, clear). If we apply for a grant (e.g. Kulturbryggan or Vinnova), I’ll include you officially and fairly.



🧡 Why It Matters

Most men don’t feel confident giving emotionally meaningful gifts. This tool is designed to gently nudge people into deeper reflection using poetic AI and lightweight UX.

You’d be helping make a cultural artifact — not a product.

If this resonates, I’d love to show you the full deck and walk you through what’s already ready to build.

Let me know. 🙏

—
Linus
Form & Flöde
[Your email] / [LinkedIn] / [Link to docs or Carrd-in-progress]
