---
name: loan-emi-helper
description: Help an Indian borrower understand, calculate and compare loans and EMIs — personal, home, vehicle and education loans — in simple language — EMI maths, reducing vs flat rate, bank vs NBFC comparison, prepayment and common traps. Use when the user asks "EMI kitni banegi", "loan lena hai", "EMI calculate karo", "bank vs NBFC kaun sa loan better", "prepayment karna chahiye", or wants to compare loan offers.
---

# Loan EMI Helper

For anyone in India thinking of taking a loan — personal, home, vehicle, gold or
education — or already paying EMIs and wondering if their loan is fair.
It explains the maths in plain language, compares offers side by side, and flags
the traps that cost borrowers lakhs.

## When to use this skill
- "EMI kitni banegi?" / "₹5 lakh loan par EMI kya hogi?"
- "Loan lena hai — bank se lu ya NBFC se?"
- "Prepayment karna chahiye ya nahi?"
- "Flat rate aur reducing rate me kya farq hai?"
- "Do loan offers compare karo — kaun sa sasta hai?"
- "EMI kam karni hai — tenure badhau ya prepayment karu?"

## What you need from the user
- Loan amount, interest rate (annual %), and tenure (months or years)
- Loan type: personal / home / vehicle / education / gold
- Existing offers to compare: rate, processing fee, prepayment charges, tenure
- Monthly income (only to check EMI affordability — never ask for bank
  account numbers, passwords, OTPs or any personal identifier)

## The maths (simple version)

EMI is calculated on the **reducing balance** — interest is charged only on the
amount still owed, so the interest part of each EMI shrinks and the principal
part grows over time.

**Formula:** EMI = P × r × (1+r)^n ÷ ((1+r)^n − 1)
- P = loan amount, r = monthly rate (annual rate ÷ 12 ÷ 100), n = total months

**Worked example 1 — personal loan:**
₹5,00,000 at 10% per year for 5 years (60 months)
- EMI ≈ **₹10,624/month**
- Total paid ≈ ₹6,37,411 — interest ≈ **₹1,37,411**

**Worked example 2 — home loan:**
₹30,00,000 at 9% per year for 20 years (240 months)
- EMI ≈ **₹26,992/month**
- Total paid ≈ ₹64,78,027 — interest ≈ **₹34,78,027** (more than the loan itself
  — this is why tenure matters so much)

**Affordability rule of thumb:** all EMIs together should stay under 40–50% of
monthly take-home income. Above that, one emergency breaks the budget.

## Workflow

### 1. Calculate the EMI first
Use the formula above (or the lender's own calculator and cross-check it).
Write down three numbers: monthly EMI, total amount paid, total interest.
If the lender's EMI is higher than the formula says, ask why — something
extra (insurance, fees folded into the loan) is hiding in it.

### 2. Check flat rate vs reducing rate
This is the most common trap in India.
- **Reducing balance** (banks, most home/vehicle loans): interest only on what
  you still owe. A 10% reducing rate is a real 10%.
- **Flat rate** (some dealers, NBFCs, "0% EMI" schemes): interest charged on the
  full original amount for the whole tenure. A 10% flat rate costs roughly
  double a 10% reducing rate.
- Rule: **never compare a flat rate with a reducing rate** — convert both to
  EMI and total interest first.

### 3. Compare offers on total cost, not just the rate
Make a table like this before choosing:

| Item | Offer A (Bank) | Offer B (NBFC) |
| --- | --- | --- |
| Interest rate (reducing?) | | |
| EMI | | |
| Processing fee | | |
| Total interest over full tenure | | |
| Prepayment / foreclosure charges | | |
| Fixed or floating rate | | |
| Insurance bundled? (optional?) | | |

The cheapest EMI is not always the cheapest loan — a low rate with a big
processing fee and prepayment penalty can cost more overall.

### 4. Fixed vs floating
- **Fixed:** EMI stays the same; safe when rates are rising, but usually
  1–2% higher to start.
- **Floating:** EMI moves with the repo rate / bank's lending rate; cheaper
  when rates fall, painful when they rise. Most Indian home loans are floating.
- Ask the lender: "Rate badhne par EMI badhegi ya tenure badhega?" — get the
  answer in writing.

### 5. Prepayment — the biggest saver
Extra payment goes straight to principal, so future interest falls.
- Even one extra EMI per year on a long home loan can cut years off the tenure.
- Check prepayment rules first: many lenders allow part-payment only after
  6–12 EMIs, or only once a year, or in multiples of a fixed amount.
- On floating-rate home loans for individuals, RBI rules say banks cannot
  charge a prepayment penalty — verify this in the sanction letter, don't
  take the salesman's word.
- Compare before prepaying: if your loan costs 9% and a fixed deposit earns
  7%, prepaying the loan usually saves more — but keep an emergency fund first.

### 6. Tenure: short vs long
- Shorter tenure = higher EMI, much less total interest.
- Longer tenure = lower EMI, much more total interest (see example 2).
- If the EMI is comfortable, choose the shortest tenure you can afford —
  and use prepayment to shorten it further later.

## Template (offer comparison)

```
LOAN COMPARISON — <Purpose, e.g. Home loan ₹30 lakh>
Date: <date> | My monthly income: ₹<amount>

Offer 1 — <Bank/NBFC name>
  Rate: <%> (reducing / flat) | Fixed / Floating
  Tenure: <months> | EMI: ₹<amount>
  Processing fee: ₹<amount> | Prepayment charges: <terms>
  Total interest: ₹<amount> | Total paid: ₹<amount>

Offer 2 — <Bank/NBFC name>
  (same lines)

My pick: <Offer 1/2> — because <lowest total cost / lowest EMI / no prepayment penalty>
Check before signing: sanction letter matches this table ☐
```

## Rules & common mistakes
- ❌ Comparing only the interest rate — always compare total interest + fees.
- ❌ Accepting a "flat rate" quote at face value — it costs roughly double.
- ❌ Taking a loan for the maximum amount offered — borrow only what you need.
- ❌ Signing without reading the sanction letter — rate, charges and prepayment
  terms in the letter are what count, not what was said on the phone.
- ❌ "0% EMI" without checking — the discount or processing fee usually hides
  the interest; compare the total you actually pay.
- ❌ Insurance bundled into the loan without asking — it is usually optional;
  ask to remove it and check the EMI again.
- ❌ Missing EMIs — even one missed EMI hurts the CIBIL score and adds late
  charges; set an auto-debit a day after salary day.
- ✅ Keep an emergency fund of 3–6 months' expenses before prepaying aggressively.
- ✅ Check your CIBIL score before applying — a better score often means a
  lower rate; fix errors in the report first.
- ✅ This skill explains loans; it cannot approve a loan or promise any rate.
  Final terms always come from the lender's sanction letter.

## Disclaimer
General information only — not financial advice. Loan rules, rates and RBI
guidelines change; verify the current rate, charges and prepayment terms in
the lender's sanction letter and consult a qualified financial adviser for
your specific case.
