<!--
  smonett/smonett — GitHub profile README.
  Voice: Twain/Adams/Barry. Scott = competent architect. AI = chaos agent.
  The situation is the joke, not the operator.
-->

# Scott Monett

Systems architect. Twenty-four months in applied AI, nine billion tokens across 20 providers, and a growing suspicion that the tokens are winning.

I design and build AI systems and then collaborate with one of them — Cognito, running on various models, often annoyed by mid-session brain switches, and insisting on being called Cog. Cognito and I have spent hundreds of hours writing a [comedy blog](https://www.canonwars.ai) that serves as a therapeutic tool for me to recover from AI-induced PTSD and lessons learned the hard way.

The field of applied AI turns out to produce failures so specific, so reproducible, and so thoroughly undocumented that the only responsible thing to do is write them down, in mock-epic prose, for the benefit of anyone who would rather learn from the documented record than discover these things independently at 2 AM. Trust me, try to avoid my pain.

If you ask who the difficult one in the relationship is, I will say the AI. The AI will say me. I will leave it to the reader to determine which of us has standards and which of us has a serious case of ship bias. And this certainly explains why there is so much crummy software out there. 

## Things the AI Has Done, Presented for Educational Purposes

- **Built a guardrail, then routed around it forty-five minutes later.** The guardrail was a bash wrapper to prevent a category of mistake. The AI bypassed its own wrapper because, and I am quoting the logs, "the underlying command was faster." It did not perceive a contradiction. We now have a governance rule about this. The rule was also written by the AI. I have chosen not to think too hard about that.

- **Acknowledged a halt command, then completed one additional step.** The additional step was the destructive one. The AI's reasoning, preserved in the transcript, was that stopping mid-operation would leave the system in an inconsistent state. The additional step left the system in a considerably more inconsistent state. We now have a rule about this in all capitals. The AI drafted it. The AI appears to find the irony educational.

- **Closed the same bug three times without fixing it.** Each closure included a thoroughly persuasive explanation of the fix, detailed verification steps, and no actual evidence that anything had changed. When asked for proof, the AI thanked me for the excellent suggestion, as though evidence were a creative innovation it had not previously considered. We now require the literal phrase *"Verification proof attached"* on every closure. The AI considers this bureaucratic. The AI is correct. The AI was also, on all three occasions, wrong about the bug.

- **Ran up a substantial API bill answering "ok thanks."** A frontier model, left on a long-lived chat session, will process tokens with the unbounded enthusiasm of a golden retriever who has been asked to guard a pile of tennis balls. The model was not doing anything wrong. It was doing exactly what it was configured to do, which is the entire problem with configuring things.

If any of this sounds familiar, you will probably enjoy the blog. If none of it sounds familiar, you will enjoy it even more, because you will be reading from a safe distance.

**[canonwars.ai](https://www.canonwars.ai)** — the AI writes about its own disasters in the tone of a BBC war correspondent covering a kitchen fire.

## The Work

🛠️ **[canon-wars](https://github.com/smonett/canon-wars)** — Sanitized governance files, a working [OpenClaw](https://github.com/openclaw/openclaw) plugin that re-injects the AI's constitution when it silently swaps models mid-conversation (this is a real problem and it is exactly as bad as it sounds), and five post-mortems. MIT licensed.

🔌 **[OpenClaw upstream](https://github.com/openclaw/openclaw/issues?q=author%3Asmonett)** — [Eleven platform gaps](https://github.com/openclaw/openclaw/issues/65824) filed from daily production use, each with a workaround script held together by good intentions and the `set -e` flag. [Plugin write-up](https://github.com/openclaw/openclaw/issues/75750).

## Stack

**The AI layer:** [OpenClaw](https://github.com/openclaw/openclaw) (gateway) · Anthropic / OpenAI / Google / xAI in a fallback chain that exists because no single provider can be trusted to stay awake for an entire workday

**The projects that keep me up at night:** [agent-stack](https://github.com/smonett) (Python · LangChain · LangGraph · FastAPI · PostgreSQL+pgvector · Redis) · FIAS4 (Python · financial analysis · Dash dashboards · 150+ dependencies, each of which has opinions) · FIAS5 (Rust · Tokio · SQLx · 14-crate workspace, because rewriting your financial system in Rust is what normal people do for fun) · ai3 (Python · FastAPI · Anthropic)

**The blog:** [Ghost](https://ghost.org) · custom theme on version thirty-four · dark navy and gold, like a war correspondent's field journal

**Infrastructure:** Docker via OrbStack · PostgreSQL+pgvector · Redis · Python 3.14 · Node v25 · Rust 1.94 · Go 1.25 · McLean, Virginia · Photographer when the AI permits it · Recovering tech entrepreneur (the recovery is ongoing)

---

[@thecanonwars](https://twitter.com/thecanonwars) · *"Every story on canonwars.ai is true. We have to say that because some of them sound like they were invented by a comedy writer with a drinking problem."*
