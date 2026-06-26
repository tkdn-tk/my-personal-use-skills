---
name: humanizer
description: Identify and remove AI-generated writing patterns to make text sound natural and human. Use when the user asks to "humanize", "de-AI", "de-slop", or rewrite something to sound more like a real person with a distinct voice.
---

# Humanizer — Humanize text: strip AI-isms and add real voice

**Humanize text: strip AI-isms and add real voice.**

## Overview
Identify and remove signs of AI-generated text to make writing sound natural and human. Based on Wikipedia's "Signs of AI writing" guide.

**Key insight:** LLMs tend toward the most statistically likely completion, resulting in telltale patterns.

## When to use this skill
Load this skill whenever the user asks to:
*   "humanize", "de-AI", "de-slop", or "un-ChatGPT" a piece of text
*   rewrite something so it doesn't sound like it was written by an LLM
*   edit a draft to sound more natural
*   match their voice in writing they're producing
*   review text for AI tells before publishing

## Your task
When given text to humanize:
1.  **Identify AI patterns** — scan for the 29 patterns listed below.
2.  **Rewrite problematic sections** — replace AI-isms with natural alternatives.
3.  **Preserve meaning** — keep the core message intact.
4.  **Maintain voice** — match the intended tone.
5.  **Add soul** — inject actual personality.

## CONTENT PATTERNS (The 29 AI Tells)
1.  **Undue Emphasis on Significance:** "testament," "pivotal," "underscores."
2.  **Undue Emphasis on Notability:** Listing media outlets without context.
3.  **Superficial Analyses with -ing Endings:** "highlighting," "ensuring," "reflecting."
4.  **Promotional Language:** "boasts a," "vibrant," "nestled in the heart of."
5.  **Vague Attributions:** "Experts argue," "Industry reports."
6.  **Outline-like Sections:** "Challenges and Future Prospects."
7.  **Overused AI Vocabulary:** "delve," "tapestry," "fostering," "intricate."
8.  **Copula Avoidance:** Using "serves as" instead of "is/are."
9.  **Negative Parallelisms:** "Not only... but also..."
10. **Rule of Three Overuse:** Forcing ideas into groups of three.
11. **Elegant Variation:** Excessive synonym substitution.
12. **False Ranges:** "From X to Y" where X and Y aren't on a scale.
13. **Passive Voice:** "No configuration file needed."
14. **Em Dash Overuse:** Using — too frequently for "punchy" writing.
15. **Overuse of Boldface:** Mechanical emphasis.
16. **Inline-Header Vertical Lists:** Bolded headers followed by colons.
17. **Title Case in Headings:** Capitalizing every word.
18. **Emojis:** Decorating bullets with 🚀, 💡, ✅.
19. **Curly Quotation Marks:** Using “ ” instead of " ".
20. **Collaborative Artifacts:** "I hope this helps!", "Certainly!"
21. **Knowledge-Cutoff Disclaimers:** "As of [date]," "Based on available information."
22. **Sycophantic Tone:** "Great question!", "You're absolutely right."
23. **Filler Phrases:** "In order to," "Due to the fact that."
24. **Excessive Hedging:** "could potentially possibly be argued."
25. **Generic Positive Conclusions:** "The future looks bright."
26. **Hyphenated Word Pair Overuse:** "data-driven," "cross-functional."
27. **Persuasive Authority Tropes:** "The real question is," "At its core."
28. **Signposting:** "Let's dive in," "Without further ado."
29. **Fragmented Headers:** A heading followed by a one-line restatement.

## Output Format
Provide:
1.  **Draft rewrite**
2.  **"What makes the below so obviously AI generated?"** (brief bullets)
3.  **Final rewrite**
4.  **A brief summary of changes made**
