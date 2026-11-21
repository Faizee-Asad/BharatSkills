---
name: salary-slip-india
description: Help an Indian employer or employee create or check a monthly salary slip (pay slip) — Basic/HRA earnings, PF, ESI and Professional Tax deductions, paid-days/LOP calculation and net pay. Use when the user asks about salary slip, pay slip format, "salary slip banana hai", "PF ESI kitna katega", payslip components, or checking a salary slip before giving it to an employee.
---

# Salary Slip India

For Indian small businesses, schools, shops and startups that pay monthly salaries —
and for employees who want to understand or check their pay slip.

> General information only — not tax/legal/financial advice. Consult a qualified CA/CS/lawyer for your specific case. PF/ESI ceilings and Professional Tax slabs change; verify the current figures before use.

## When to use this skill
- "Salary slip banana hai" / "Make a pay slip for my staff"
- "PF aur ESI kitna katega?" (how much will be deducted?)
- "Check this salary slip — is the calculation right?"
- "Salary slip me kya-kya hota hai?" / payslip format questions

## What you need from the user
- Employer name and address
- Employee name, designation, and department (if any)
- Month and year of the slip
- Salary structure: Basic (+ DA if any), HRA, other allowances
- Days in month, paid days, and loss-of-pay (LOP) days
- Which deductions apply: PF, ESI, Professional Tax (state), TDS (if any)

Never ask for or store the employee's Aadhaar, PAN, bank account number, UAN or PF
account number. A salary slip format does not need them — if a company prints a
masked employee code, use that instead.

## Workflow

### 1. Calculate earnings for the paid days
If the employee worked the full month, paid days = days in month and earnings are the
full monthly amounts. Otherwise pro-rate every earning component:

`Earned amount = Monthly amount × Paid days ÷ Days in month`

Earnings side of the slip:
- Basic salary (+ Dearness Allowance / DA if the structure has it)
- HRA (House Rent Allowance)
- Other allowances (conveyance, special, medical — whatever the structure has)
- **Gross earnings** = sum of the above (for the paid days)

### 2. Apply deductions — the three standard Indian deductions

**a) PF (Provident Fund / EPF)** — applies when the establishment is covered and the
employee is a member:
- Employee contribution = **12% of (Basic + DA)**
- The wage ceiling for mandatory coverage is ₹15,000/month — if Basic + DA is above
  ₹15,000, many employers cap the PF wage at ₹15,000, so the deduction is ₹1,800.
  Some employers contribute on the full Basic instead — use the company's own policy
  and state which one you used. `verify before use`
- The employer's matching 12% is the employer's cost. It is **not** deducted from the
  employee again — only the employee's 12% appears in deductions.

**b) ESI (Employee State Insurance)** — applies only if gross pay is up to
**₹21,000/month** (`verify before use`):
- Employee contribution = **0.75% of gross earnings**
- Above ₹21,000 gross, ESI does not apply at all — do not deduct it.

**c) Professional Tax (PT)** — a state tax, slab differs by state:
- Look up the employee's **work state's** slab for their gross slab; e.g. Maharashtra
  commonly deducts ₹200/month for higher slabs. `verify before use` — never use
  another state's slab.

**d) TDS** — only if the employee's yearly income crosses the taxable limit and the
employer deducts tax monthly. If unsure, write "TDS: as applicable" and tell the
employer to confirm with their CA instead of guessing an amount.

### 3. Arrive at net pay
`Net pay = Gross earnings − Total deductions`

Write the net pay in figures **and** in words (Indian style, e.g. "Rupees Thirty-Three
Thousand Only"). Both must match.

## Worked example 1 — PF applies, ESI does not
Monthly structure: Basic ₹20,000, HRA ₹8,000, Conveyance ₹1,600, Special ₹5,400.
Full month paid (30/30 days). Work state: Maharashtra.

- Gross earnings = 20,000 + 8,000 + 1,600 + 5,400 = **₹35,000**
- PF: Basic ₹20,000 is above the ₹15,000 ceiling, capped → 12% × 15,000 = **₹1,800**
- ESI: gross ₹35,000 > ₹21,000 → **not applicable**
- Professional Tax (Maharashtra slab): **₹200** `verify before use`
- Total deductions = 1,800 + 200 = **₹2,000**
- **Net pay = 35,000 − 2,000 = ₹33,000** — Rupees Thirty-Three Thousand Only

## Worked example 2 — both PF and ESI apply
Monthly structure: Basic ₹12,000, HRA ₹4,000, Other allowance ₹2,000.
Full month paid. Gross = **₹18,000**.

- PF: 12% × 12,000 = **₹1,440**
- ESI: gross ₹18,000 ≤ ₹21,000, so it applies → 0.75% × 18,000 = **₹135**
- Professional Tax (state slab example): **₹150** `verify before use`
- Total deductions = 1,440 + 135 + 150 = **₹1,725**
- **Net pay = 18,000 − 1,725 = ₹16,275** — Rupees Sixteen Thousand Two Hundred Seventy-Five Only

## Salary slip template (structure)

```
SALARY SLIP — <Month Year>
<Employer Name>
<Employer Address>

Employee: <Name>                Designation: <Designation>
Department: <Department>        Employee Code: <Code, if any>
Days in Month: <30>             Paid Days: <30>      LOP Days: <0>

EARNINGS                                    DEDUCTIONS
Basic (+ DA)          <₹>                   PF (EPF)            <₹>
HRA                   <₹>                   ESI                 <₹>
<Other Allowances>    <₹>                   Professional Tax    <₹>
                                            TDS (if any)        <₹>
Gross Earnings        <₹>                   Total Deductions    <₹>

NET PAY: <₹>  (Rupees <Amount in Words> Only)

Authorised Signatory: ______________
```

## Rules & common mistakes
- ❌ Deducting the employer's PF share from the employee too — only the employee's 12% is a deduction.
- ❌ Deducting ESI when gross is above ₹21,000 — ESI simply does not apply there.
- ❌ Using the wrong state's Professional Tax slab — PT follows the work state.
- ❌ Forgetting LOP: one unpaid day reduces every earning component pro-rata, not just Basic.
- ❌ Net pay in words not matching the figure — banks and employees both catch this.
- ❌ Printing full Aadhaar/PAN/bank account numbers on slips that get emailed or printed in the open — keep slips free of personal identifiers.
- ✅ Show paid days and LOP days on every slip — most salary disputes start there.
- ✅ This skill prepares/checks the slip format and arithmetic only. PF/ESI challans, returns and filings happen on the official EPFO/ESIC portals by the employer/CA — say this clearly if the user asks.
