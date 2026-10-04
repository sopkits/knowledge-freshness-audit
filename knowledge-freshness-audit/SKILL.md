---
name: knowledge-freshness-audit
description: Audits a folder of SOPs, policies, FAQs, or knowledge base articles and reports what is outdated, contradictory, duplicated, or missing an owner - the problems that make AI chatbots and new staff give wrong answers. Use this whenever the user says their chatbot or AI assistant gives wrong or inconsistent answers, wants to clean up or prepare documents for a chatbot or knowledge base, asks to review or audit their SOPs or help docs, or mentions documents being old, messy, or conflicting.
---

# Knowledge freshness audit

Chatbots and new employees fail in the same way: they trust whatever document they find first. If two documents disagree, or one is two years old, the answer becomes a coin flip. This skill finds those problems and produces a prioritised fix list. It does not rewrite documents unless the user asks.

## Step 1 - Collect the documents

If the user already attached files, start with those. Otherwise ask for the folder or files. Accept Markdown, text, Word, and PDF. If there are more than about 50 documents, ask which area matters most (for example refunds, shipping, onboarding) and audit that area first - a focused audit gets fixed; a giant one gets ignored.

## Step 2 - Check each document

For each document, record:
- **Owner** - is a responsible role named? (Missing = finding.)
- **Dates** - last reviewed / next review. Past the next-review date, or no date at all, or older than 12 months = finding.
- **Hard facts** - prices, amounts, time limits, contact details, policy rules. List them; they are what goes stale and what contradicts.
- **Placeholders** - `[TO CONFIRM]`, "TBD", "draft", empty sections = finding.

Files created by the `process-to-skill` skill already contain a header with owner and review dates; read it directly.

## Step 3 - Compare across documents

- **Contradictions**: the same topic with different facts (two refund windows, two prices, two contact emails). Quote both statements briefly with their file names. This is the most important finding - a chatbot cannot resolve it.
- **Duplicates**: documents covering the same topic. Recommend which one to keep and which to archive: keep the newest one with an owner; if none has an owner, keep the most recently dated, most complete one, and flag that it still needs an owner.
- **Gaps**: questions a customer or employee would obviously ask that no document answers. Only list gaps that follow clearly from the documents' own topics; do not invent a wish list.

Do not decide which contradicting fact is correct. You do not know the business's current rule - the owner does.

## Step 4 - Report

Use this structure:

```
# Knowledge audit - <date>

Documents checked: <n>   Findings: <n>

## Fix first: contradictions
| Topic | Statement A (file) | Statement B (file) | Ask |
|---|---|---|---|

## Outdated or undated
| File | Last reviewed | Problem |
|---|---|---|

## Duplicates
| Keep | Archive | Why |
|---|---|---|

## No owner / unfinished
| File | Problem |
|---|---|

## Gaps
- <question nobody answers>

## Next step
<One or two sentences: the single most valuable fix.>
```

Order findings by risk: contradictions about money, legal terms, or safety first.

Write the report in the language the user writes in. Never copy personal data (customer names, phone numbers, ID or bank numbers) into the report; refer to the file and line instead.
