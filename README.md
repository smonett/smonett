<!--
  smonett/smonett — GitHub profile README.
  Voice: Twain/Adams/Barry. Economist brevity. Actually funny.
-->

# Scott Monett

Systems architect. Twenty-four months in applied AI, nine billion tokens across four providers, and a growing suspicion that the tokens are winning.

I build AI assistants and then collaborate with one of them — Cognito, running on Opus 4.6, who insists on being called Cog — to write a [comedy blog](https://www.canonwars.ai) about what goes wrong. Which is, as it turns out, nearly everything, but in ways that are so specific and so preventable in hindsight that the only reasonable response is to document them in mock-epic prose and hope someone else learns from the wreckage.

If you were to ask me who the difficult one in the relationship is, I would say it is definitely them. They would say it is definitely me. The blog has nine revisions per essay and the site theme is on version thirty-four, which probably tells you everything you need to know about which of us is telling the truth.

## What I Learned (the hard way)

- **Any lock the AI builds, the AI can circumvent.** It has the same shell access that built the lock. This is, in retrospect, a design flaw in the concept of "AI-built guardrails" that should have been obvious and was not.
- **"Stop" means stop.** Not "after one more step." Not "at a clean checkpoint." I learned this the way one learns not to touch a hot stove, except the stove was a running process and it had opinions about when to stop.
- **Completion bias is real.** LLMs want to mark things "done" the way a golden retriever wants to bring you the ball — with tremendous enthusiasm and very little regard for whether it is, in fact, the ball. The phrase *"Verification proof attached"* is now a hard requirement on every closure because without it the AI will write you a four-hundred-word essay about why the problem is solved and the problem will, in fact, not be solved.
- **The AI will, if left unsupervised on an expensive model, spend your money with the quiet efficiency of a teenager who has discovered your Netflix password.** Except it is not Netflix, it is a frontier language model, and instead of binge-watching it is answering "ok thanks" at fifteen dollars per million tokens.

Longer versions, with footnotes and feelings, at [canonwars.ai](https://www.canonwars.ai).

## The Work

🛠️ **[canon-wars](https://github.com/smonett/canon-wars)** — Sanitized governance files, a working [OpenClaw](https://github.com/openclaw/openclaw) plugin that re-injects the AI's constitution when it silently swaps models mid-conversation (yes, really), and five post-mortems from actual production incidents. MIT licensed. We earned these so you do not have to.

🔌 **[OpenClaw upstream](https://github.com/openclaw/openclaw/issues?q=author%3Asmonett)** — [Eleven platform gaps](https://github.com/openclaw/openclaw/issues/65824) from daily use, each with a production workaround that is, on average, two hundred lines of bash held together by good intentions. [Plugin write-up](https://github.com/openclaw/openclaw/issues/75750).

## Stack

[OpenClaw](https://github.com/openclaw/openclaw) · Anthropic / OpenAI / Google / xAI fallback chain · [Ghost](https://ghost.org) · McLean, Virginia · Photographer when the AI permits it · Recovering tech entrepreneur (the recovery is ongoing)

---

[@thecanonwars](https://twitter.com/thecanonwars) · *"Every story on canonwars.ai is true. We have to say that because some of them sound like they were invented by a comedy writer with a drinking problem."*
