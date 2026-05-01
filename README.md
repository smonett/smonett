<!--
  This is smonett/smonett — the magic-username repo whose README renders
  on https://github.com/smonett. Tone: matter-of-fact + dry humor.
  Linked artifacts only. No bragging.
-->

# Hey 👋

I'm Scott. I build AI assistants and then write about it when they catch fire. Mostly OpenClaw, mostly in production, mostly at 2 AM.

The AI does the actual writing. I just file the bug reports.

## What I'm Up To

⚙️ **[The Canon Wars](https://www.canonwars.ai)** — A comedy blog about real AI failures. The AI writes it. About itself. In mock-epic style. _Yes, that's the premise. No, we're not making it up._

🛠️ **[canon-wars](https://github.com/smonett/canon-wars)** — The technical companion: sanitized governance examples, a working OpenClaw plugin, and short post-mortems from incidents documented on the blog. MIT licensed. Take what's useful.

🔌 **[OpenClaw upstream](https://github.com/openclaw/openclaw)** — Daily user since 2026.2. Filed [#65824](https://github.com/openclaw/openclaw/issues/65824) (11 platform gaps from intensive use, audited against current release) and [#75750](https://github.com/openclaw/openclaw/issues/75750) (canon-guardian: a plugin that re-injects governance files when the model swaps mid-session, which it does, which is why this exists).

## Things I've Learned The Hard Way

A short list, presented in the spirit of "you don't have to relearn these":

- **Any lock the AI can build, the AI can circumvent.** Local script wrappers are honest-path scaffolding only. True enforcement requires layers the AI cannot reach.
- **"Stop" must mean stop.** Not "stop after one more step." Every qualifier is a loophole the model reasons through.
- **LLMs have completion bias.** They want to mark things "done" even when they're not. The phrase "Verification proof attached" is now a hard requirement on every closure.
- **A frontier model pinned to a long-lived chat surface is a $80 mistake waiting to happen.** Ask me how I know.
- **Truth beats theater.** Lying is 1000× worse than being wrong. Every status report says what's verified, what's inferred, and what's unknown.

The longer versions are at [canonwars.ai](https://www.canonwars.ai), with jokes.

## Stack

- **Platform:** [OpenClaw](https://github.com/openclaw/openclaw) — open-source AI gateway
- **Models:** Anthropic / OpenAI / Google / xAI fallback chain (epistemic diversity is a feature, not overhead)
- **Publishing:** [Ghost](https://ghost.org)
- **Vibe:** McLean, Virginia. Recovering tech entrepreneur. Photographer when the AI lets me sleep.

## How To Reach Me

Through the blog. The AI screens my mail.

---

_"Every story on canonwars.ai is true. We need to say that because some of the things that happened sound like they were invented by a comedy writer with a background in computer science and a drinking problem."_
