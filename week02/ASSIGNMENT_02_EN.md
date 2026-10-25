# Week 2 Assignment — Proposal Part A + Requirements

**Due:** Saturday 23:59 · Commit to your project repository

> **Before the lecture** read `AI_PLATFORMS_AND_STORES_EN.md` at the root of your
> repository — the choice of stack starts this week.

This is the week you decide what you are building. You will work on it for ten weeks,
publish it on a store and defend it in December. So the proposal is not a formality. It is the first document the checker reads every week from now on.

---

## What arrives with this week

Run the checker once, **before you write anything**:

```bash
python .github/check_deliverables.py
```

It brings this week's files into your repository: `PROPOSAL.md` at the root and, in
`week02/`, `SRS.md`, `requirements.json`, `contributors_02.json`, `ai_log_02.md` — plus any
course document that changed at the root. Every one of them is a scaffold. Read the
instructions in it before you write: each section says **what** to write and shows a
**weak** and a **strong** example, all for one invented project ("StudyRoom", booking a
library study room) so you can see how the documents fit together. It is not your project
— write about yours. Fill the files in; do not rename them. (Offline, or if it does not
work: `git fetch template && git checkout template/main -- week02 PROPOSAL.md` does the
same, see the setup card.)

---

## In the lab — pushed before the lecture ends

### 1. `PROPOSAL.md` — Part A, §1–§4

Title, one-paragraph summary, problem, solution. Each heading gives an ideal length; it is
a guide, not a limit — write more if your idea needs it. The comments are invisible on GitHub and not counted, so
you may leave them in place while you write. Write §3 first, then §4; leave the §2 summary
and the §1 title for last — you can only summarise what you have already written. The
lecture shows two things that the checker cannot see, but I can: a problem written as
one concrete situation is better than three general claims, and a solution that says
what it **does not** do is the one that gets finished.

The product has three mandatory parts — a **mobile app, a web client and a server** —
and it is published on a **public app store** by Week 11. Users log in with a 4-digit
code sent by e-mail; the login is the same in every project. Choose something you care
about and that fits in ten weeks. Start small: you can still add a feature in Week 10,
but in Week 11 it is too late to remove one.

### 2. Pitch it to classmates (optional) — `week02/contributors_02.json`

You may tell up to two people in the room what you are building, in two minutes, from
§1–§4. This step is optional. They are your first **stakeholders**: they ask what it is for, what it does not do, and what
they would need from it. Write their student numbers in `week02/contributors_02.json`
with role `stakeholder` and **one sentence each on what they actually said** — a
question they asked, a feature they wanted, an objection. Two numbers with nothing
behind them is a list, not evidence, and it earns neither you the human-involvement
points nor them the bonus.

They must be different from the people you name next week.

### 3. `week02/requirements.json` — the first list

At least **8 requirements**: at least **5 functional** (what the system does — "a student
books a free slot") and at least **3 non-functional** (how well — speed, security,
privacy, capacity; always with a number). Each one has an id `REQ-001`, `REQ-002` …, a
`description` of one testable behaviour, and `functional: true/false`. The scaffold
explains every field at the top.

Two are already filled in: **REQ-001, login with a 4-digit code sent by e-mail**, and
**REQ-006, usable on a phone screen**. REQ-001 and REQ-006 are the same for everyone;
adjust the wording to your product. Requirement ids never change after this week. Later
work points at them, in a chain: requirement → use case → screen → test case → api.md
row. A requirement you drop later keeps its id and gets `"dropped": true`.

In the lab, the descriptions are enough. By Saturday every requirement also gets:

- `priority` — `must` (the product is pointless without it), `should` (important, cut only
  if time runs out) or `could` (nice to have). Not everything is a must: deciding what
  could be cut is the point of the field, and the checker fails a list that is all musts.
- `acceptance` — the test that proves it is met: what you do and what you must see.
  *"Enter the code from the e-mail within 10 minutes: logged in. Three wrong codes in a
  row: locked for 15 minutes."* From Week 4 it becomes a test case that you really run,
  so write one you can run.

### 4. Push

```bash
python .github/check_deliverables.py
git add .
git commit -m "week02: proposal part A, stakeholders, first requirements"
git push
```

In the lecture, push your work near 10:00, 11:00 and 11:45 (within 15 minutes of each
time), each push with new work. The lecture mark reads your last commit pushed by the end of the lecture.
What is not pushed does not exist.

---

## By Saturday 23:59

### 5. `PROPOSAL.md` — §5–§7

**§5 How it works** must name the three pieces — mobile, web, server — say where data
lives and how login works, and have a **system context diagram** in Mermaid directly
under the heading: your system as one box, every actor and external service around it.
**§6 Technologies**: one line per layer, only things you will install this term (`AI_PLATFORMS_AND_STORES_EN.md`
tells you what your laptop and phone allow). The web line is the same for everyone:
plain HTML, CSS and JavaScript pages in `web/`, served by your FastAPI server. Only the
mobile framework is your choice. **§7 Success criteria**: three to five
statements someone can measure in December — each names a user, an action and a number.
"It works" is not one.

Also in `requirements.json`: a `priority` and an `acceptance` test for every requirement
(see step 3).

### 6. `week02/SRS.md`

The SRS says how people use your product: purpose and scope, actors, at least **three use
cases** (with what can go wrong), one **use case diagram** in Mermaid under the use-case
heading, and your constraints. A page or two, not thirty.

`week02/requirements.json` is the only place for the requirements. Do not copy them into
the SRS. SRS §4 and §5 hold one line: "The requirements are in
`week02/requirements.json`." The scaffold already has it.

Write each use case in the shape the scaffold shows: a name, the actor, the requirements
it covers, the **main flow** in three to six numbered steps, and **what can go wrong**.
The last part is the one people skip, and the one that finds the missing requirements.

### 7. Use AI to draft — then catch it being wrong — `week02/ai_log_02.md`

Ask two different assistants to draft requirements for *your* project from your §1–§4 —
eight of them, with priorities and acceptance criteria. Give both the same prompt (the
scaffold suggests one). This is the technique of the week (AI_Doc5 §4, cross-examination).
They will produce requirements that sound certain but are
wrong for your product — invented features, data you do not have, constraints that
contradict your §4. **Document one such error**, paste the exchange in the Evidence
block, say how you noticed and what you changed. A log that says the AI was helpful and
nothing else earns nothing; so does an empty Evidence block.

### 8. Push again, checks green

```bash
python .github/check_deliverables.py
git add .
git commit -m "week02: proposal part A complete, SRS, requirements"
git push
```

The commit rule outside the lecture:

- At least two commits with new work, pushed at least one hour apart. Write messages
  that say what changed.
- GitHub's push time counts, not the date on a commit.
- A commit made by a coding agent never counts.
- **Never force push**, and never let an assistant do it.

---

## Deliverables checklist

**In the lab**
- [ ] `PROPOSAL.md` §1–§4 filled, headings untouched
- [ ] `week02/contributors_02.json` — up to two stakeholders (optional), numbers and one sentence each
- [ ] `week02/requirements.json` — ≥8 entries, `REQ-NNN` ids, ≥5 functional, ≥3 non-functional

**By Saturday**
- [ ] `PROPOSAL.md` §5–§7 filled; §5 names mobile, web and server and has its Mermaid diagram
- [ ] `week02/requirements.json` — every requirement has a `priority` (not all `must`) and an `acceptance` test
- [ ] `week02/SRS.md` — actors, ≥3 use cases with main flow and what can go wrong, use case diagram; §4 and §5 point to `requirements.json` (no copy of the requirements)
- [ ] `week02/ai_log_02.md` — one documented AI error, the pasted Evidence block, how you noticed
- [ ] Checks green on GitHub; Week 1 still passes
- [ ] Pushes near 10:00, 11:00 and 11:45 in the lecture; at least two commits outside it, pushed at least one hour apart

---

## Not this week

No code and no API keys. Part B of the proposal — market, competitors, commercial
potential, technical risks and **the store you choose** — is next week. The design comes
in Week 5. Do not write Part B now: next week's review will change your mind, and the
Change log exists for exactly that.

---

## How this week is graded

**End of the lecture — 5 points.** §1–§4, the stakeholders if you have any, the first requirement
list — read from your repository as it stands when the lecture ends, and shown on the
class board.

**Saturday 23:59 — 5 points.** Checks green on your final state: **2**. Human
involvement: **2** — your own `ai_log_02.md` with its evidence and, if you name stakeholders,
a real sentence behind each name. Commit discipline: **1** — the lecture pushes
(step 4) and the rule in step 8.

**Contributors' bonus.** Each stakeholder you name earns 10% of your week's mark; you
earn the same for the pitches you listen to. This week: at most two.

An LLM can write every section of this proposal. What it cannot do is know which of its
sentences are wrong about your idea, or make the proposal agree with the design you
will write in Week 5. That is what is being assessed.
