# Input / Output

**A single-session behavioural experience for upper-school English.**

Students read a source text, write a response, and submit it. What they read back is not quite what they wrote. A debrief reveals what changed — and why.

---

## What it does

The tool runs in four screens:

1. **Read** — A source text covering four real cases of data use without meaningful consent: the Facebook emotional contagion experiment (2012), Cambridge Analytica's psychological profiling operation (2016), and corporate voice recording programmes. No company names are given. The legal status of each case is stated.

2. **Write** — Students type a free response (minimum 60 characters). While they type, a drift engine monitors for sentence-ending pauses and applies up to two invisible substitutions to their text. The substitutions move language toward certainty, compliance, and institutional register — removing hedges, flattening affect, neutralising resistance vocabulary.

3. **Review** — Students read back what was submitted. The text looks like theirs. A secondary drift fires after five seconds, altering one further word silently.

4. **Debrief** — A "Continue" button reveals what happened. If substitutions occurred, each is shown as a before/after pair with word-level diff highlighting. If no substitutions occurred — because the student's phrasing didn't match any drift patterns — that outcome is stated directly, which is worth discussing in its own right.

Five discussion questions follow the diff display.

---

## The drift logic

The substitution rules fall into four categories:

- **Hedge removal** — `I think I` → `I`, `I suppose` → `I accept`, `maybe I` → `I`, `a bit` → *(deleted)*
- **Certainty enforcement** — `I think` → `I know`, `I feel` → `I acknowledge`, `seems` → `is`
- **Register shift** — `weird` → `significant`, `disturbing` → `relevant`, `wrong` → `inconsistent`, `manipulation` → `direction`
- **Counter-directional rules** — occasional reversals (`I know` → `I think I know`) that break any pattern a student might try to detect

Substitutions fire at sentence-completion pauses (1.8 seconds after `.`, `!`, or `?`) and on blur before submit. The cursor position is preserved. Nothing changes visibly.

---

## Classroom use

**Recommended:** individual devices, no discussion until the debrief screen.

**Time:** 20–35 minutes including discussion.

**The no-change outcome** is pedagogically useful. A student whose text wasn't altered can discuss: *Why not? What does that say about how I wrote — and about how these systems target language?*

**Do not pre-explain the drift mechanic.** The experience depends on students not knowing.

---

## Abitur Themenfeld relevance

| Themenfeld | Angle |
|---|---|
| Science & Technology | Algorithmic systems, behavioural data, utopia/dystopia |
| The Individual & Society | Autonomy, consent, the construction of the compliant subject |
| Politics, Culture & Society – USA | Cambridge Analytica, election interference, platform governance |

---

## Deployment

Single HTML file. No dependencies, no server, no data is collected or transmitted. Drop `index.html` into any GitHub Pages repository.

To rename for deployment: rename `working-title.html` to `index.html` before pushing.

---

## Discussion questions (included in the debrief screen)

1. You did not notice the changes while they were happening. What does that tell you about how systems — digital or institutional — can operate on you without your awareness?
2. The substitutions moved your language toward certainty and compliance. Who benefits when uncertainty and hesitation are removed from public expression?
3. This system used your own words as its raw material. How is that different from simply replacing what you wrote with something else entirely?
4. The companies described in the source text were, in most cases, operating legally. Does legality settle the ethical question?
5. What would it mean to genuinely consent to this — and is meaningful consent possible when the system is invisible?
