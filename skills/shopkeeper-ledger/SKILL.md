---
name: shopkeeper-ledger
description: Help an Indian shopkeeper keep a simple daily sales and udhaar (credit) ledger — cash, UPI and credit sales, daily cash tally, udhaar recovery and ageing, weekly summary. Use when the user asks about dukaan ka hisaab, "shopkeeper ledger banana hai", daily sales record, udhaar khata, "cash tally nahi mil raha", or tracking who owes the shop money.
---

# Shopkeeper Ledger

For Indian kirana shops, general stores and small dukaan owners who keep the
day's hisaab in a notebook, a register, or a simple sheet — no accounting
software needed.

> General information only — not tax/legal/financial advice. This skill keeps
> a daily sales and credit record; GST billing and tax filing are separate and
> need a CA or the gst-invoice-helper skill.

## When to use this skill
- "Dukaan ka roz ka hisaab rakhna hai" / "Make a daily ledger for my shop"
- "Udhaar khata banana hai" / who owes the shop, and how much
- "Cash tally nahi mil raha" — closing cash does not match the day's sales
- "Week ka total sales kitna hua?" / weekly or monthly summary
- "Udhaar wapas kaise maangu?" — polite recovery reminders

## What you need from the user
- Shop name (optional — for the ledger heading)
- The day's sales split: cash sales, UPI sales, udhaar (credit) sales
- Opening cash in the galla / drawer at the start of the day
- Any udhaar recovery received today (old credit paid back, cash or UPI)
- Day's expenses: stock purchase, transport, shop kharcha
- For udhaar entries: customer name, amount, date — and phone number only if
  the customer agreed to reminders

Never ask for or store Aadhaar, PAN, bank account numbers or OTPs. A shop
ledger needs only names, amounts and dates — never a customer's ID or bank
details.

## Workflow

### 1. Record the day's sales in three columns
Every sale goes in exactly one column — never in two:

- **Cash** — customer paid notes/coins at the counter
- **UPI** — paid by PhonePe / GPay / Paytm (check the app's daily total at
  closing; the app total and the ledger must match)
- **Udhaar** — goods given on credit, to be paid later; write the customer
  name in the udhaar khata the same day, never "yaad se"

`Total sales of the day = Cash sales + UPI sales + Udhaar sales`

### 2. Tally the cash at closing (galla milao)
Count the cash in the drawer and compare it with what the ledger says
should be there:

`Expected cash = Opening cash + Cash sales + Udhaar recovery (cash) − Cash expenses`

- If counted cash is **less** than expected → cash is short: re-count, check
  whether a cash sale was written in the UPI column by mistake, or whether an
  expense was paid from the drawer without writing it down.
- If counted cash is **more** than expected → cash is extra: check whether a
  UPI sale was written as cash, or an old udhaar recovery was counted twice.
- Write the difference down every day, even if it is small. A ₹100 shortfall
  ignored daily becomes ₹3,000 in a month.
- UPI money does **not** sit in the drawer — never add UPI sales to the cash
  tally. Check UPI separately against the app.

### 3. Keep the udhaar khata (credit book)
One page per regular customer: date, goods/amount given, amount paid back,
balance left. Update it the same day — udhaar forgotten is udhaar lost.

`Customer balance = All udhaar given − All payments received`

Age every balance so old udhaar does not hide:
- **0–7 days** — fresh, normal
- **8–30 days** — remind politely once a week
- **30+ days** — talk to the customer in person; stop new udhaar until the
  old balance is cleared or a part payment is made

Never give new udhaar to a customer whose 30+ day balance is growing. The
rule protects the shop and the friendship both.

### 4. Close the week and the month
Add the 7 daily totals for a weekly summary, and the daily totals for a
monthly summary:

- Total sales (cash + UPI + udhaar), total recovery, total expenses
- Udhaar outstanding at week/month end — how much customers owe in total,
  and how much of it is 30+ days old
- Cash short/excess for the week — if the same shortfall repeats, look for
  the pattern (same time of day, same person at the counter, same expense)
- Once a month, count the stock of the fastest-moving 10 items and compare
  with the ledger — sales without stock falling means entries are missing

## Worked example 1 — one day, cash short by ₹150
Opening cash in galla: ₹2,000. Day's sales: cash ₹18,450, UPI ₹12,300,
udhaar ₹3,750. Old udhaar recovery received in cash: ₹1,500. Expenses:
₹1,200 (stock ₹800 + shop kharcha ₹400).

- Total sales = 18,450 + 12,300 + 3,750 = **₹34,500**
- Expected cash at closing = 2,000 + 18,450 + 1,500 − 1,200 = **₹20,750**
- Counted cash in drawer: ₹20,600 → **short by ₹150**
- Action: write "short ₹150" in the ledger, re-count once, check whether the
  ₹400 kharcha was written down — if the shortfall repeats tomorrow, check
  the counter routine, not the arithmetic.
- Udhaar outstanding grew by 3,750 − 1,500 = **₹2,250** today.

## Worked example 2 — one week summary
7 days. Cash sales ₹1,12,400, UPI sales ₹78,900, udhaar sales ₹21,300.
Udhaar recovery ₹9,800. Expenses ₹14,600. Opening cash on Monday: ₹3,000.

- Total week sales = 1,12,400 + 78,900 + 21,300 = **₹2,12,600**
- Expected cash on Sunday closing = 3,000 + 1,12,400 + 9,800 − 14,600
  = **₹1,10,600** (check this against the counted cash; UPI ₹78,900 is
  in the bank/app, not in the drawer)
- Udhaar outstanding grew by 21,300 − 9,800 = **₹11,500** this week — if
  most of it is in the 30+ day bucket, next week's first job is recovery,
  not new udhaar.

## Daily ledger template

```
ROZ KA HISAB — <Date> — <Shop Name>
Opening cash (galla): ₹<...>

SALES
Cash sales:   ₹<...>
UPI sales:    ₹<...>
Udhaar sales: ₹<...>
TOTAL SALES:  ₹<...>

RECOVERY (purana udhaar wapas)
<Customer Name>: ₹<...> (cash/UPI)

EXPENSES
<Stock / Transport / Kharcha>: ₹<...>
TOTAL EXPENSES: ₹<...>

CASH TALLY
Expected cash = Opening + Cash sales + Cash recovery − Cash expenses = ₹<...>
Counted cash in drawer: ₹<...>
Difference: ₹<...> (short / extra / mil gaya ✓)

UDHAAR KHATA — aaj ke entries
<Customer Name> — ₹<...> — Balance: ₹<...>
```

## Weekly summary template

```
WEEK — <Mon Date> to <Sun Date>
Total sales: ₹<...> (Cash ₹<...> + UPI ₹<...> + Udhaar ₹<...>)
Total recovery: ₹<...>    Total expenses: ₹<...>
Udhaar outstanding: ₹<...> (0–7 days ₹<...> | 8–30 days ₹<...> | 30+ days ₹<...>)
Cash short/excess this week: ₹<...>
Top 3 udhaar customers to remind: <Name — ₹...>, <Name — ₹...>, <Name — ₹...>
```

## Polite udhaar reminder (Hinglish)

```
Namaste <Name> ji, aapka <₹Amount> ka hisaab <Date> se baki hai.
Jab time mile to de dena, koi jaldi nahi. Dukaan par aakar ya UPI se
bhej sakte hain. Dhanyavaad 🙏 — <Shop Name>
```

## Rules & common mistakes
- ❌ Writing the same sale in two columns (cash + UPI) — the day's total
  inflates and the cash tally never matches.
- ❌ Adding UPI sales to the drawer cash tally — UPI money is in the
  bank/app, not in the galla.
- ❌ Writing udhaar "yaad se" later — write the name and amount the same
  day, or it will be forgotten.
- ❌ Giving new udhaar while a 30+ day balance is unpaid and growing.
- ❌ Ignoring a small daily shortfall — write it down; patterns only show
  up in the written record.
- ✅ Close the ledger every night: tally cash, check the UPI app total,
  update the udhaar khata — 10 minutes a day beats a month of guessing.
- ✅ Keep one notebook/register only for the shop — personal kharcha in the
  same book is the commonest reason tallies never match.
- ✅ This skill is a record-keeping format, not accounting software. If the
  shop is GST-registered, GST bills and returns still follow the shop's CA
  and the gst-invoice-helper skill.
