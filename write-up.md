# Daily Reflection Tree — Design Write-Up

**Assignment:** DT Fellowship | The Daily Reflection Tree  
**Part A:** Deterministic Tree Structure

---

## Why These Questions

The central challenge in this assignment is not technical — it's **epistemological**: how do you write a question that genuinely surfaces a psychological state, without leading the respondent or shaming them?

Each axis demanded a different approach:

### Axis 1: Locus of Control

The opening question — "Give today one word" — is deceptively structural. The four options (Productive, Draining, Mixed, Frustrating) split cleanly into emotionally positive/neutral vs. emotionally negative, which determines the first branch. This matters because someone who says "Frustrating" needs a different follow-up than someone who says "Productive" — not because one is better, but because **the lens shifts**. A person on a good day needs to examine whether they're attributing success to internal factors. A person on a bad day needs to find the small moments of agency they may be dismissing.

The follow-up questions avoid the word "control" deliberately — because asking someone "did you feel in control?" primes a socially desirable response. Instead, we ask for *behaviors* ("What was your first move?") which are harder to rationalize post-hoc.

### Axis 2: Orientation (Contribution vs. Entitlement)

This axis is the hardest to surface honestly because **entitlement is invisible to the person holding it.** No one thinks of themselves as entitled. So the questions approach it obliquely:

- "What was your primary feeling going into that interaction?" (intent, not outcome)
- "Did you feel the world owed you something today?" (blunt, but framed as a genuine question)

The branching here tries to catch the person who initially signals contribution but is actually looking for recognition ("I wanted to help" → "Did you get what you were hoping for?"). That path leads toward honest self-examination rather than self-congratulation.

### Axis 3: Radius of Concern

Maslow's late-career insight — that self-transcendence sits above self-actualization — is underappreciated because it sounds abstract. The tree makes it concrete: **who came to mind while you were in the problem?** This is a behavioral proxy for radius of concern. Naming a colleague, a customer, or an end user is an act of perspective-taking that you either did or didn't do.

The options are ordered from narrow (just me) to wide (end user) — not to shame the narrow response, but to make the spectrum visible.

---

## Branching Trade-offs

**Trade-off 1: Depth vs. Completion Rate**  
Longer trees are more revealing but more likely to be abandoned. I targeted 6-9 interactions per session, with a hard maximum of ~12 nodes per path. This required making decision nodes "invisible" (auto-advance) so users only interact with question and reflection nodes.

**Trade-off 2: Signal Purity vs. Real-world Messiness**  
Real human responses are not cleanly "internal" or "external." The tree includes a `mixed` signal track on every axis precisely to avoid forcing false dichotomies. A person who partially self-identified with both sides of a question routes to a "mixed" reflection — which is often the most honest outcome.

**Trade-off 3: Fixed Options vs. Authentic Expression**  
Free text would be more authentic but unprocessable. The solution is to make the fixed options **feel like they could have been things you'd actually say** — not abstract psychological descriptors ("I exhibited internal locus behavior") but concrete behavioral moments ("I looked for something I could control"). The test I used: would a real person at 7pm recognize themselves in at least one of these?

---

## Psychological Sources

| Concept | Source | Application |
|---|---|---|
| Locus of Control | Rotter, J.B. (1954) | Core structure of Axis 1 |
| Growth Mindset | Dweck, C. (2006), *Mindset* | Informs the reframe in A1 reflections |
| Psychological Entitlement | Campbell et al. (2004) | Core structure of Axis 2 |
| Organizational Citizenship Behavior | Organ, D.W. (1988) | Contribution-side options in Axis 2 |
| Self-Transcendence | Maslow, A. (1969) | Core structure of Axis 3 |
| Perspective-Taking | Batson, C.D. (2011) | Question design for Axis 3 |

---

## What I'd Improve With More Time

1. **Adaptive question weight.** If a user answers identically on all three axes across multiple sessions, the tree should offer a variant question path — not to trick them, but because familiarity breeds autopilot.

2. **Longitudinal summary.** After 5 sessions, a "pattern view" that shows how the user's axis distributions shift over time. This is the difference between a reflection *tool* and a reflection *practice*.

3. **Tone calibration by axis result.** Currently all reflections have the same warm-but-direct tone. A user consistently scoring "external/entitlement/self" across sessions may benefit from a slightly more challenging reframe — not shaming, but not purely validating either.

4. **The opening question is too abstract.** "Give today one word" works but "Productive/Draining/Mixed/Frustrating" may not capture days that are *anxious*, *boring*, or *exciting*. A richer initial taxonomy would improve the first branch's fidelity.

5. **Collaboration testing.** The questions should be tested against real users in cognitive walkthroughs — not to find the "right" answers, but to identify where the options feel strained or where people feel none of the options fits them.

---

*Total nodes: 40+ | Question nodes: 14 | Decision nodes: 12 | Reflection nodes: 9 | Bridge nodes: 2 | Summary/End: 2*
