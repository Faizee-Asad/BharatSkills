# Contributing to BharatSkills

Thank you for being here. This project grows one skill at a time — exactly the way
other contributors (including the maintainer) started in open source: one small,
useful, well-checked addition.

**You do not need to be a programmer.** A skill is a single Markdown file.
If you know how a real Indian workflow works — fees, GST, typing exams, farming,
a shop's ledger — you already know enough to contribute.

---

## The fastest way to contribute: pick a missing skill

These skills are wanted and **do not exist yet**. Each one is a ready-made first PR.
Claim one by opening an issue first (so two people don't build the same skill),
then follow the steps below.

### 🔴 HIGH priority — Business & Finance
- [x] `salary-slip-india` — salary slip + payroll prep with PF / ESI / Professional Tax
- [x] `shopkeeper-ledger` — daily sales / udhaar (credit) ledger format for small shops
- [x] `freelancer-proposal-india` — proposal + quotation for Indian clients, UPI / milestone payment terms
- [ ] `dpdp-basics` — DPDP Act privacy basics checklist for small businesses (general info only)

### 🔴 HIGH priority — Language & Government
- [x] `hindi-typing-helper` — Kruti Dev ↔ Unicode workflow, government typing-exam context
- [ ] `govt-form-helper` — how to read a government form and build a document checklist (public process only — never collect personal IDs)
- [ ] `hinglish-content-writer` — Hinglish ad / social copy for Indian businesses

### 🟡 Wanted — Education
- [x] `exam-planner-india` — GATE / SSC / UPSC / state-exam study and score planning
- [ ] `school-timetable-helper` — period / timetable planning for Indian schools
- [ ] `result-sheet-helper` — marksheet / result summary in school formats

### 🟡 Wanted — Everyday India
- [ ] `wedding-planner-india` — Indian wedding planning checklist (functions, guests, vendors)
- [ ] `farmer-helper-india` — mandi price, season and scheme information workflow (general info only)
- [ ] `rent-agreement-helper` — reading a rent agreement, common clauses checklist (general info only)
- [ ] `train-journey-planner-india` — Indian Railways journey planning (PNR, waitlist, tatkal concepts)

### 🟢 Also welcome
- A translation of an existing skill into Hindi, Marathi, Bengali, Tamil, Telugu,
  Gujarati, Punjabi, Kannada, Malayalam or any Indian language
- A fix: a wrong GST rule, a better template, a clearer example
- A new category we haven't thought of — open an issue and propose it

---

## How to add a skill (step by step)

1. **Fork** this repository.
2. **Copy the template folder:**
   ```
   skills/_template/  →  skills/<your-skill-name>/
   ```
   Skill names: lowercase, hyphens, no spaces (e.g. `school-fee-reminder`).
3. **Edit `SKILL.md`** inside your folder. Fill every section of the template.
   Keep it practical: real steps, real templates, real examples.
4. **Add one line** for your skill in `docs/skills.md` (same table format).
5. **Add a CHANGELOG entry** under `## [Unreleased]` in `CHANGELOG.md`.
6. **Open a Pull Request** to `main`. Use the PR template — it has a small checklist.

That's it. The maintainer will review, suggest small fixes if needed, and merge.

## Skill quality rules (please read — PRs are checked against these)

1. **No personal data, ever.** Never ask the user for Aadhaar, PAN, bank details,
   passwords, OTPs or any identifier. If a workflow normally involves an ID,
   describe the *process* only and tell the user to enter it only on the official site/app.
2. **No invented law or tax rules.** If you state a GST rate, a deadline or a legal
   requirement, be sure of it — or clearly mark it `verify before use`.
   Tax/legal/finance skills must carry this line:
   *"General information only — not tax/legal/financial advice. Consult a qualified CA/CS/lawyer for your specific case."*
3. **Real templates, not theory.** Every skill must include at least one copy-ready
   template or example a user can use immediately.
4. **Explain the Indian context.** Don't assume the reader knows what UPI, GSTIN,
   Kruti Dev or a mandi is — one line of explanation is enough.
5. **Simple language.** Short steps. English is fine; Hinglish/Hindi examples are a bonus, not a burden.
6. **One skill, one job.** If your idea does two unrelated things, split it into two skills.

## What gets rejected

- Skills copied from another project without credit / licence compatibility
- Skills containing real people's names, phone numbers, IDs or private data
- Spam, promotional or affiliate content
- Medical diagnosis / treatment skills (out of scope for this project)

## Review & merging

- Every PR gets a reply — if something needs a fix, we'll tell you exactly what, in simple words.
- Small, correct PRs merge fastest. One skill per PR, please.

## Code of Conduct

Be kind, be patient, assume good intent. Many contributors here are first-timers —
help them the way you would have wanted to be helped on your first PR.
