# BharatSkills 🇮🇳

**India-first AI agent skills for Claude Code, Codex, Cursor and other Agent Skills-compatible tools.**

A drop-in skill bundle that teaches your AI assistant how work actually happens in India — GST invoices, UPI payments, WhatsApp Business conversations, school fees, Hindi typing, Indian exams, PF/ESI payroll, and government paperwork.

> Most agent skill libraries are built for the US: US tax, US payroll, US invoices.
> An audit of ~84,700 community agent skills found **zero native Hindi skills**.
> BharatSkills fills that gap — built in India, for India, open to everyone.

## Why this exists

- Anthropic's official Small Business plugin covers US workflows (US tax prep, US payroll) — it has no GST, no UPI, no WhatsApp Business, no DPDP.
- Global tool/skill collections have no Kruti Dev, no GATE/SSC workflows, no Indian school workflows.
- Indian SMBs, freelancers, teachers, CAs and students deserve AI skills written for *their* reality — in English, Hinglish and Hindi.

## What's inside (v0.1.0)

| Category | Skill | What it does |
|---|---|---|
| Business & Finance | `gst-invoice-helper` | GST invoice structure, CGST/SGST vs IGST logic, HSN/SAC summary, common mistakes |
| Business & Finance | `upi-payment-followup` | Polite-to-firm UPI payment reminders in English / Hinglish / Hindi |
| Business & Finance | `salary-slip-india` | Indian salary slip format — PF/ESI/Professional Tax deductions, paid-days/LOP calculation, worked examples |
| Business & Finance | `loan-emi-helper` | Loan & EMI maths in simple language — reducing vs flat rate, bank vs NBFC total cost, prepayment rules |
| Business & Finance | `shopkeeper-ledger` | Daily sales & udhaar ledger for small shops — cash/UPI/credit columns, closing cash tally, udhaar ageing |
| Business & Finance | `dpdp-basics` | DPDP Act privacy basics for small businesses — consent & notice, retention & deletion, children's data, breach plan |
| Business & Communication | `whatsapp-business-writer` | WhatsApp replies, offers, order updates and follow-ups the way Indian customers actually chat |
| Business & Communication | `festival-offer-planner` | Festival offers and campaigns for Indian shops — Diwali, Eid, Rakhi, Onam — timeline, honest offers, ready messages |
| Education | `school-fee-reminder` | Respectful fee reminders for parents — English / Hindi / Marathi templates, receipt follow-ups |
| Education | `school-admission-helper` | Admission enquiries, parent replies, document checklists and follow-ups for schools |
| Education | `exam-planner-india` | GATE/SSC/UPSC study planning — days-and-hours maths, syllabus weight split, mock analysis, revision cycles |
| Education | `hindi-typing-helper` | Kruti Dev ↔ Unicode conversion workflow, font/layout choices, government typing-exam preparation |
| Career & Jobs | `resume-fresher-india` | Fresher resume for Naukri/LinkedIn/Internshala — structure, objective, projects, ATS-friendly format |
| Career & Jobs | `freelancer-proposal-india` | Client proposals & quotations for Indian freelancers — scope, milestones, advance and UPI payment terms |
| Everyday India | `marriage-biodata-maker` | Marriage biodata formats — traditional, Muslim and modern short formats in Hindi/English |
| Everyday India | `traffic-challan-helper` | Check, pay or contest a traffic e-challan safely — official Parivahan portal only, fake-SMS scam protection |

**Coming soon (help wanted — see [CONTRIBUTING.md](CONTRIBUTING.md)):**
`exam-planner-india` · `freelancer-proposal-india` · `dpdp-basics` · `shopkeeper-ledger` · `govt-form-helper` · `hinglish-content-writer` · and 12+ more listed as good-first-issues.

Full searchable catalog → [docs/skills.md](docs/skills.md)

## Install

### Claude Code (plugin marketplace)
```
/plugin marketplace add Faizee-Asad/BharatSkills
```

### Manual (any agent that supports Agent Skills)
Copy any skill folder into your skills directory:

```bash
git clone https://github.com/Faizee-Asad/BharatSkills.git
cp -r BharatSkills/skills/gst-invoice-helper ~/.claude/skills/
cp -r BharatSkills/skills/upi-payment-followup ~/.claude/skills/
```

Then just ask naturally — *"GST invoice banana hai, inter-state sale hai"* or *"client ko UPI payment ka polite reminder bhejo"* — the right skill loads automatically.

## How a skill works

Each skill is one folder with one `SKILL.md` file — plain Markdown, no code required.
That means **anyone can contribute**: a teacher can add a school workflow, a CA can add a GST workflow, a shopkeeper can add a ledger format. If you can write steps in simple language, you can ship a skill.

## Contributing

We *want* your skill. See [CONTRIBUTING.md](CONTRIBUTING.md) for:
- The **HIGH-priority missing skills list** (pick one, it's a ready-made first PR)
- A copy-paste skill template
- Simple rules: no personal data, no fake/incorrect legal or tax claims, mark anything you are unsure about

New contributors: look for issues labelled `good first issue`.

## Principles

1. **India-first, not India-only** — every skill explains the Indian context so any user (or AI) can follow it.
2. **Privacy first** — skills must never ask for or store Aadhaar numbers, PAN, bank passwords, OTPs or any personal identifiers.
3. **Honest limits** — tax/legal skills carry a clear disclaimer: general information only, consult a CA/CS/lawyer for your specific case.
4. **Language is a feature** — English, Hinglish and Hindi examples are welcome. A skill that a Malegaon shopkeeper can use beats one only a Bangalore startup can.

## Maintainer

Built and maintained by **Asad Faizee** ([@Faizee-Asad](https://github.com/Faizee-Asad)) — Noor Infotech, Malegaon, Maharashtra.

## License

MIT — see [LICENSE](LICENSE). Use it, fork it, ship it.

---

⭐ If this helps you, star the repo — it helps other Indian builders find it.
