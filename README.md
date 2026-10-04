# Knowledge Freshness Audit - free Claude skill

**Your AI chatbot gives wrong answers? Check the documents behind it.**

Chatbots and new employees fail the same way: they trust whatever document they find first. If two documents disagree, or one is two years old, the answer becomes a coin flip.

This free Claude skill audits your SOPs, policies, FAQs, or help articles and gives you a prioritised fix list:

- **Contradictions** - the same topic with different facts (two refund windows, two support emails)
- **Outdated or undated** documents
- **Duplicates** - which to keep, which to archive
- **No owner / unfinished** documents (TBD, drafts, empty answers)
- **Gaps** - obvious questions nobody answers

It never decides which contradicting fact is correct - your business does. And it never copies personal data into the report.

## Try it in 2 minutes

1. Download `knowledge-freshness-audit.skill` and click **Save skill** in Claude (or upload it in Claude's Skills settings). Requires a Claude plan that supports Skills.
2. Attach your documents and say: **"Audit these help docs - our chatbot keeps giving wrong answers."**

See `example/` for a test run: 4 small documents with planted problems, and the report the skill produced.

Claude Code users: copy the `knowledge-freshness-audit/` folder into your skills directory.

## Want to fix the problem at the source?

The audit finds what's broken. The **[Process-to-Skill Kit](https://sopkits.gumroad.com/l/process-to-skill-kit)** writes it right the first time: explain a process once, and get an SOP for your team, a Claude skill for your agent, and a chatbot-ready knowledge base article with an owner and review date - all from one conversation. Includes this audit skill.

## License

MIT - free to use, modify, and share. Not affiliated with Anthropic.
