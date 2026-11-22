---
name: traffic-challan-helper
description: Help an Indian vehicle owner check, understand, pay or contest a traffic e-challan — in simple language — verify a challan on the official Parivahan portal, pay it safely, dispute a wrong challan through grievance / Virtual Court / Lok Adalat, and spot fake challan SMS scams. Use when the user asks "challan check karo", "challan kaise bhare", "galat challan aaya hai", "challan SMS aaya hai — sahi hai ya fake", or wants to know what happens if a challan is left unpaid.
---

# Traffic Challan Helper

For anyone in India who got a traffic challan — or an SMS saying they have
one — and wants to know: is it real, how much is it, how do I pay it, and
what if it is wrong? It walks through the official route only, so the user
never pays a scammer by mistake.

## When to use this skill
- "Mera challan check karo" / "Gaadi par koi challan hai kya?"
- "Challan kaise bharu?" / "Challan online pay karna hai"
- "Galat challan aaya hai — kya karu?"
- "Challan wala SMS aaya hai, sahi hai ya fake?"
- "Challan nahi bhara to kya hoga?" / "Gaadi bechni hai, challan pending hai"
- "Court me challan gaya hai — ab kya karna hai?"

## What you need from the user
- Vehicle registration number (e.g. MH-41-AB-1234), OR challan number, OR
  driving licence number
- For a vehicle-number search, the last 4 digits of the chassis number or
  engine number (the portal asks for this to confirm ownership)
- What the SMS / notice says: amount, date, place, offence — if they have it

Never ask for Aadhaar, PAN, bank account numbers, passwords or OTPs. The
official portal never asks for these through a call, SMS or message link —
anyone who does is a scammer.

## The official route (only this one)

**Check / pay — Parivahan e-Challan portal:**
`echallan.parivahan.gov.in` — type this address yourself in the browser,
never open a link that arrived by SMS or WhatsApp.
- "Check Challan Status" → search by challan number, vehicle number or
  driving licence number → enter captcha → "Get Detail"
- The record shows the offence, date, place, amount and — for camera
  challans — the photo evidence. Check the photo: is it your vehicle, your
  number plate, the right date and place?
- To pay: "Pay Now" → UPI, debit/credit card or net banking → save the
  receipt and transaction ID, and re-check the status after payment to
  confirm it shows as paid.
- The same check/pay works in the official **mParivahan** app.
- Some states run their own portal alongside Parivahan — for example,
  Maharashtra uses `mahatrafficechallan.gov.in`. The challan SMS or paper
  notice usually names the system that issued it; use that portal only if
  the challan does not appear on Parivahan. (Verify the state portal
  address on the state traffic police site before paying.)
- Maharashtra note: the national portal now routes MH-registered vehicles
  to the NextGen portal `echallan.parivahan.nic.in` — if a challan does
  not appear on the older `echallan.parivahan.gov.in`, check NextGen and
  the Maharashtra portal too, but pay each challan only once, in one place.
- Maharashtra — Abhay Yojana 2026 (verify before promising it): the state
  cabinet approved on 4 Nov 2026 a one-time discount of up to 20% on
  pending compoundable challans, in three phases — but no notification/GR
  had been published by that night. Tell the user to check the official
  portal for whether the scheme is live for their challan, and warn them
  that SMS/WhatsApp messages offering "20% off, pay at this link" are a
  scam pattern — never pay through such a link.

## Workflow

### 1. Verify first — pay second
- Open the portal yourself and search. If the challan is **not there**,
  do not pay anything from the SMS link — treat the message as suspicious
  (see step 4).
- Match the details: vehicle number, date, time, place, offence and photo.
  Camera challans (speed, red light, ANPR) usually have a photo; a
  hand-written challan issued on the road may not.
- Payment is an admission that the challan is correct — so if anything
  looks wrong, do **not** pay first. Dispute it instead (step 3).

### 2. If the challan is correct — pay and keep proof
- Pay on the official portal (step above) and download the receipt.
- Re-check the status after payment — it should show as paid/closed.
- Keep the receipt until the challan disappears from the pending list;
  it is the proof if the same challan ever resurfaces.
- Unpaid challans do not just vanish: they can pile up, go to court, and
  cause trouble later with RC renewal, ownership transfer or fitness
  certificate work. Check pending challans before selling a vehicle.

### 3. If the challan is wrong — contest it, don't just ignore it
- **Grievance first:** on the Parivahan e-Challan portal, use the
  complaint/grievance section — describe what is wrong (wrong vehicle,
  wrong number plate read by camera, you were not at that place on that
  date) and attach the proof you have (photo, RC, location proof). Keep
  the acknowledgement number.
- **If it has gone to court:** the challan moves to Virtual Court
  (`vcourts.gov.in`) — open the case there, choose "I wish to contest
  the case", confirm with OTP and submit. You will get the court name
  and date; the case then moves to a regular court.
- **Lok Adalat:** pending challans can often be settled at a Lok Adalat
  at a reduced amount — check the dates for your district's Lok Adalat
  (National Lok Adalat dates are announced by NALSA / the district
  legal services authority). This is a settlement, not a contest — use
  it when the challan is broadly correct but you want a lower fine.
- Keep every acknowledgement, receipt and court date in one place — the
  template below helps.

### 4. Fake challan SMS — the scam check
Red flags — treat the message as fake until proven otherwise:
- It asks you to pay through a link in the SMS/WhatsApp, or to a personal
  UPI ID / unknown app.
- It pressures you ("pay in 2 hours or licence will be cancelled") or asks
  for an OTP, password or bank details.
- The amount or vehicle does not match, or the portal shows no such challan.

What to do:
- Do **not** click the link and do **not** pay. Type
  `echallan.parivahan.gov.in` yourself and search — a real challan will
  be listed there.
- If no record exists, report it: call the cybercrime helpline **1930**
  or report at `cybercrime.gov.in`, and forward the SMS as evidence.
- Real challan SMS comes as an information message — it never asks you to
  share an OTP or pay to a personal UPI ID.

## Templates

### Challan record (keep one per challan)
```
CHALLAN — <Vehicle number>
Challan no.: <number> | Date: <date> | Place: <place>
Offence: <e.g. overspeeding / red light / no helmet>
Amount: ₹<amount> | Photo evidence: Yes / No — matches my vehicle? Yes / No
Status: Correct — pay / Wrong — contest / SMS only, no portal record — fake?
Paid on: <date> | Receipt / transaction ID: <id>
Grievance / court ref: <number> | Next date: <date>
```

### Message to send after paying (WhatsApp, to self/family record)
```
Challan bhara — <Vehicle number>, ₹<Amount>, challan no. <number>.
Receipt save kar li hai. Portal par status "paid" dikh raha hai.
```

### Grievance text (short, copy-ready)
```
Subject: Wrong e-challan — <Challan no.>, vehicle <number>

Sir/Madam,
Mujhe challan no. <number> dated <date> mila hai, offence <offence>,
place <place>. Ye challan galat hai kyunki <reason — e.g. photo me
meri gaadi nahi hai / us date par gaadi us jagah thi hi nahi>.
Sahi details: <vehicle no., date, place>. Proof attached hai.
Kripya is challan ko correct/dispose karein.
<Name>, <Mobile>, <Vehicle no.>
```

## Rules & common mistakes
- ❌ Paying from an SMS/WhatsApp link — always type the portal address
  yourself.
- ❌ Paying first and disputing later — payment usually closes the case
  as admitted; check the facts before paying.
- ❌ Ignoring a challan — it can go to court and block RC-related work
  later.
- ❌ Sharing OTP, password or bank details for a "challan payment" —
  the government never asks for these.
- ❌ Trusting a fine amount from memory or a forwarded message — fine
  amounts differ by state and offence; use only the amount on the
  official record.
- ✅ Check the photo evidence before deciding pay vs contest.
- ✅ Save the receipt and re-check the status after payment.
- ✅ Keep challan number, grievance number and court date together.

## Disclaimer
General information only — not legal advice. Traffic fines, procedures and
portals differ by state and change over time; verify the current process on
the official portal for your state, and consult a qualified lawyer for a
case that has reached court.
