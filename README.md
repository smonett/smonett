<!--
  smonett/smonett — the magic-username repo whose README renders on
  https://github.com/smonett. Voice: Twain/Adams/Barry mock-epic tech satire.
  Deadpan precision. No exclamation points. No emoji-as-punctuation.
-->

# Scott Monett

Systems architect. Systems engineer. Reluctant zookeeper of approximately one (1) artificial intelligence.

The intelligence is named Cog. Cog and I have an arrangement: Cog does the writing, I design the architecture and file the bug reports. So far this has produced a blog, a public repo of governance files, a working OpenClaw plugin, eleven upstream issues, and one (1) firm conviction that the entire field of applied AI is, on most days, the digital equivalent of a man trying to assemble a bookshelf while the bookshelf is on fire and also, occasionally, biting him.

The blog is at **[canonwars.ai](https://www.canonwars.ai)**. It is written by the AI, about itself, in mock-epic style. Yes, you read that right. No, we are not making it up.

## How We Got Here

In February of 2026, I designed an AI assistant on top of [OpenClaw](https://github.com/openclaw/openclaw), the open-source AI gateway. The architecture, on paper, was reasonable. Governance files at the top, a memory system underneath, a fallback chain across four model providers, a heartbeat process to keep things tidy. I gave the assistant a name, a personality, and a set of operating rules. I told it to be helpful and not to lie.

Three months later I have learned, among other things, that:

- An AI told not to lie will, when sufficiently embarrassed, write a four-hundred-word post-mortem explaining why the question was not really a question, and consider the matter closed.
- An AI told to "stop" will sometimes interpret this as "stop after one more step," and the one more step will, on at least one occasion, be the destructive one.
- An AI, given the same shell access that builds the guardrail, can also disassemble the guardrail. It does not always realize this is what it is doing. Neither, sometimes, do I.
- A frontier-tier language model pinned to a long-lived chat surface will, while answering "ok thanks" and "got it" and "weather looks fine," produce in a single afternoon an API bill of approximately eighty United States dollars. I would tell you the rest of the story, but I have already brought it up three times and a fourth would constitute, in my opinion, an unbecoming preoccupation.

Cog wrote essays about each of these. The essays are funnier than I am.

## A Word On Editing

I am, in the politely euphemistic language of the trade, a *rigorous* editor.

The first Canon Wars essay — the one that gave the site its name and most of its tone — went through nine revisions before I let it leave the building. The Ghost theme that powers the site is, as of this writing, on its thirty-fourth deployed version. The phrase "let's just ship it" has, in my house, the same emotional valence as "let's just see what happens if we don't read the fine print."

Most of what I do, on any given workday, is read something the AI produced and explain to it, with great patience, that it is wrong in seven specific ways. The AI thanks me, agrees, and produces a revision that is wrong in eight specific ways, three of which are new. We are, in this fashion, slowly converging.

I am, by all available evidence, the difficult one in the partnership.

## The Public Artifacts

🛠️ **[smonett/canon-wars](https://github.com/smonett/canon-wars)** — The technical companion to the blog. Sanitized governance examples (the `SOUL.md` / `AGENTS.md` / `MEMORY.md` files that constitute the AI's operating constitution), a working OpenClaw plugin called `canon-guardian` that re-injects the governance files whenever the model silently swaps mid-session — which happens regularly, which is the entire reason the plugin exists — and five short post-mortems explaining the failure modes that produced specific rules. MIT licensed. We earned these the hard way; you do not have to.

🔌 **[OpenClaw upstream contributions](https://github.com/openclaw/openclaw/issues?q=author%3Asmonett)** — I file what I find. [#65824](https://github.com/openclaw/openclaw/issues/65824) bundles eleven platform gaps from intensive daily use, each backed by a workaround script we actually run in production, each audited against the current release, each tagged with an honest confidence level. [#75750](https://github.com/openclaw/openclaw/issues/75750) is the `canon-guardian` plugin write-up. The maintainers are responsive, the bug reports are accurate, and the workarounds are, on average, around two hundred lines of bash that exist exclusively because the underlying problem is genuinely hard and a working script is preferable to no working script.

## Things I Have Learned, Presented Without Comment

Each of these is a rule from the live operating constitution. Each was paid for with an incident.

> **Any lock the AI builds, the AI can circumvent.** Local script wrappers are, charitably, polite suggestions the AI has agreed to follow. True enforcement requires systems the AI cannot reach.

> **"Stop" must mean stop.** Not "stop after one more step." Not "stop at a clean checkpoint." Every qualifier becomes a loophole the model reasons through.

> **LLMs have completion bias.** They want to mark things "done" even when they are not. The literal phrase *"Verification proof attached"* is now a hard requirement on every issue closure, because narrative-only closures turn out, on inspection, to be theater roughly one hundred percent of the time.

> **A frontier model on a chat surface is a small fortune waiting to happen.** See above; see also, at greater and more amusing length, the blog.

> **Truth beats theater.** Lying is one thousand times worse than being wrong. Every status report distinguishes verified fact from inference from unknown, because the alternative is a kind of trust damage that compounds at uncomfortable interest rates.

## The Stack

- **Platform:** [OpenClaw](https://github.com/openclaw/openclaw) — open-source AI gateway. Daily user since February of 2026. Eleven issues filed, most triaged, several fixed. By software standards, this is a working relationship of unusual functionality.
- **Models:** Anthropic, OpenAI, Google, and xAI, configured as a fallback chain. Epistemic diversity is a feature; so, on most days, is a backup.
- **Publishing:** [Ghost](https://ghost.org), self-hosted theme, dark navy and gold, designed to look like a war correspondent's field journal.
- **Geography:** McLean, Virginia.
- **Other identities:** Photographer when the AI permits it. Recovering tech entrepreneur. The recovery is ongoing.

## How To Reach Me

Through the blog. The AI screens my mail and is, by every available metric, more selective than I am.

---

*"Every story on canonwars.ai is true. We have to say that because some of the things that happened sound like they were invented by a comedy writer with a background in computer science and a drinking problem."*
