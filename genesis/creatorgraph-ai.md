# CreatorGraph AI — Startup Genesis

**Date:** 2026-05-07
**Founder:** Rajesh Ranjan
**Status:** Pre-build. Idea validated in founder's own mind. MVP not started.

---

## The One-Line Definition

A memory-first content intelligence platform that builds a living knowledge graph of a creator's past content, audience reactions, private signals, and competitor landscape — so every content decision starts from evidence, not instinct.

---

## How the Idea Evolved — The Real Conversation

This is not the polished pitch. This is the genesis session, captured raw.

### The Original Framing (Wrong)
Started as: *"AI content strategist for creators."*
Problem: every tool already claims that. Competitive graveyard.

### The First Real Insight
The actual differentiator: **continuity**.

> Creators do not need another blank prompt box. They need a system that knows what they have already said, what their audience responded to, what was rejected, and what should become a sequel.

Most tools have no memory. Every session starts from zero. That is the gap.

### The Aha Moment (The Real Product)

The unlock moment that makes this irreplaceable:

> **Before you start on a new idea, it tells you: "You explored this exact concept on March 3rd. You abandoned it because of these reasons. Here is what you knew then."**

This is not a content tool. This is **institutional memory for a solo founder**. The thing every solo founder loses because it lives in their head and their head forgets.

Every person who has kept a journal, a Notion doc, a voice memo at 2am has tried to solve this. They all fail because retrieval is broken. You find the thing only after you've already made the mistake again.

### The Validation Layer (Second Insight)

Before investing hours creating content, the system looks at historical evidence and answers: **"Is this content strategy even worth pursuing today?"**

Most tools answer: *"How do I write this?"*
CreatorGraph answers: *"Should I even write this?"*

That is a completely different and more valuable question.

If you want to rerun the validation — it will. Markets shift. Audiences evolve. A topic validated six months ago might be dead now or finally ready.

### The Three Layers That Stack

```
Layer 1 — Memory:     "You thought about this before. Here's what you knew."
Layer 2 — Validation: "Here's whether this is even worth your time today."
Layer 3 — Execution:  "Here's the transcript in your voice."
```

Most tools only have Layer 3. Nobody has all three.

---

## The Knowledge Graph — Four Memory Sources

Each source answers a different question. Together they build a complete picture.

| Source | What it answers | Ingestion method |
|--------|----------------|-----------------|
| **YouTube / TikTok / Instagram / LinkedIn** | What you said publicly and how it performed | API + creator data exports |
| **Own documents / notes / talks** | Your unfiltered thinking and ideas | Upload: markdown, PDF, text |
| **Email sent folder** | What expertise you gave away privately. What your audience asked 47 times but you never addressed publicly | One-time historical export. Process, extract patterns, discard raw data. |
| **Competitor + market** | What's already been said. Where the gap is. | Creator-provided competitor handles |

### On Email — The Precise Scope
Email is **only for building the past knowledge graph**. Not ongoing monitoring. Not inbox management. Creator exports their own archive once. System reads it, extracts patterns, builds the graph, stores only the graph — not the raw messages. Creator stays in control. Raw data never lives on servers permanently.

### On WhatsApp / Private Signals
Same principle — private signals are the richest content source (people ask you what they REALLY want to know in DMs, not in comments). Process with strict privacy constraints:
- On-device processing only, OR
- Creator manually shares specific messages they choose, OR
- Strict anonymisation before anything touches servers

---

## The Cold Start Solution

**No waiting 90 days to build history.**

Day one ingestion:
1. Creator's own archive (past posts, documents, emails)
2. Competitor public content (provided by creator)
3. Market signals

The validation layer is rich from day one — not just against the creator's own history but against the entire competitive landscape.

**Data network effect:** As more creators in the same niche use CreatorGraph, the competitor and market graph becomes richer for everyone. The product gets smarter as the community grows.

---

## Platform Priority

| Platform | Priority | Why |
|----------|----------|-----|
| YouTube | First | Richest data: transcripts + performance + comments in one API pull |
| Own documents | First | Karpathy LLM Wiki layer. Accepts any markdown, PDF, text |
| LinkedIn | High | Highest willingness to pay. Daily posters feel repetition pain most acutely |
| TikTok | Medium | Creator data export. Rich for short-form creators |
| Instagram | Medium | Creator data export |
| Email (historical) | Onboarding | One-time past knowledge graph ingestion |
| WhatsApp | Later | Private signals, handle with strict privacy design |

---

## MVP Architecture

Inspired by Karpathy's LLM Wiki pattern (April 2026):
> "Skip the vector DB. Pre-compile knowledge into structured markdown. LLM reads it directly. Synthesis is done once — not re-derived every query."

**MVP Stack:**
- Markdown files, not graph databases
- Direct context injection into LLM — no RAG
- One LLM call to answer "what have I been circling around that I haven't built yet?"
- Append-only event log (dated entries, never overwrite history)
- No Neo4j. No LangGraph. No pgvector. Not yet.

**Prove the memory value first. The architecture catches up later.**

---

## The Build Plan

### Week 1 — Prove it to yourself
Start a daily markdown log. Every idea. Every abandoned thread. Every "I thought about this but..." — one file, append-only, dated entries.

After 30 days: ask Claude to read the whole file and answer:
*"What have I been circling around that I haven't built yet?"*

If that answer is useful — that's the product.

### Step 2 — Three other creators
Not a beta. Not a waitlist. Three people you know personally who create content. Sit with them. Watch where they lean in. Three sessions > three months of solo building.

### Step 3 — First paying customers
Not VCs. Ten potential customers. Ask them to pay. Even $99. A credit card is the only real validation. Enthusiasm is cheap.

---

## The Unfair Advantage

- Rajesh is the first customer (EdTech founder, frequent content creator, LinkedIn thought leader)
- Deep Claude Code + gstack expertise — can build the MVP in a weekend using the very principles being taught
- Context Engineering tutorial series = distribution for the product
- **The tutorial and the product are the same thing**

Build CreatorGraph AI as the capstone project of the Context Engineering tutorial series. Show people how to build their own creator memory system. Then offer to run it for them.

---

## Open Questions (Unresolved at Genesis)

1. **Who is the highest-value paying customer without LinkedIn?** (Resolved: LinkedIn is back in)
2. **Agency play** — creator agencies (10-50 creators) = B2B wedge. Higher ARPA. Rethinking priority.
3. **LinkedIn ingestion** — API is painful. Best path: creator's own data export from LinkedIn settings.
4. **Pricing model** — not defined yet. Likely tiered: solo creator / agency.
5. **Where does "market" signal come from?** — RSS, newsletters, podcast transcripts. Needs tighter definition.

---

## Competitive Position

> **The competitive wedge: CreatorGraph AI does not promise "viral scripts." It promises "creator-original strategy from your own memory."**

The best answer is not another generic idea. It is the next logical move in the creator's body of work.

No competitor combines:
- Historical memory (not just recent content)
- Private signals (email, DMs) as content intelligence
- Validation layer (should I even do this?)
- Competitor gap analysis from stored graph

---

## The Founding Insight (One Sentence)

> Your best post is sitting in your sent folder right now. You wrote it at 11pm to one person who asked a good question. Nobody else ever saw it.

---

## References

- Andrej Karpathy, LLM Wiki (April 2026): [gist.github.com/karpathy/442a6bf555914893e9891c11519de94f](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f)
- Karpathy, LLM OS: context window = RAM, model weights = CPU, external storage = disk
- Logseq: graph-based, local-first, markdown knowledge management — inspiration for the graph structure
- CreatorGraph AI Detailed Design & Market Research (internal doc, May 2026)

---

*This document was written on 2026-05-07 as a genesis memory — the founding session of the idea. When the company exists, read this first.*
