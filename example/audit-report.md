# Knowledge audit - 2026-10-03

Documents checked: 4   Findings: 8

## Fix first: contradictions
| Topic | Statement A (file) | Statement B (file) | Ask |
|---|---|---|---|
| Return/refund window | 7 days after delivery (refund-policy.md, returns-old.md) | 14 days (faq.md) | Which window applies today? |
| Support contact | support@shop.example (refund-policy.md) | help@shop.example (faq.md) | Which address is monitored? |

## Outdated or undated
| File | Last reviewed | Problem |
|---|---|---|
| refund-policy.md | 2024-11-02 | Older than 12 months; no next-review date |
| faq.md | none | No review date |
| returns-old.md | none | No review date |

## Duplicates
| Keep | Archive | Why |
|---|---|---|
| refund-policy.md (after fixing) | returns-old.md | Same rule, returns-old.md has no date or owner |

## No owner / unfinished
| File | Problem |
|---|---|
| refund-policy.md | No owner |
| faq.md | No owner; "TBD" answer for international shipping |
| returns-old.md | No owner |

## Gaps
- Do you ship abroad? (faq.md raises it but no document answers it)

## Next step
Decide the real refund window and support email, update one document, and archive returns-old.md - a chatbot currently has a 50/50 chance of quoting the wrong window.
