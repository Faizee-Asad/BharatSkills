---
name: gst-invoice-helper
description: Help an Indian business create or check a GST tax invoice — correct CGST/SGST vs IGST split based on place of supply, GSTIN format, HSN/SAC summary, invoice numbering and common GST mistakes. Use when the user asks about GST invoice, billing with GST, "GST bill banana hai", "invoice me GST kaise lagau", inter-state vs intra-state tax, or checking an invoice before sending it.
---

# GST Invoice Helper

For Indian businesses, freelancers and accountants who need a correct, complete
GST invoice — or want to check one before sending it to a customer.

> General information only — not tax/legal/financial advice. Consult a qualified CA/CS/lawyer for your specific case. GST rates and rules change; verify the current rate for your HSN/SAC before issuing.

## When to use this skill
- "GST invoice banana hai" / "Make a GST bill for a client in another state"
- "CGST/SGST lagega ya IGST?" (which tax split applies?)
- "Check this invoice — is anything missing?"
- "HSN summary kya hota hai?" / invoice format questions

## What you need from the user
- Seller name, address, state and GSTIN (format check only — never store it)
- Buyer name, address, state and GSTIN (if B2B; not needed for a B2C retail invoice)
- Items/services: description, HSN (goods) or SAC (services), quantity, rate, GST rate %
- Invoice number and date, place of supply (the state where the buyer is located / service is received)

Never ask for passwords, OTPs, or login details for the GST portal. This skill only
prepares/checks the invoice content — filing happens by the user/CA on official channels.

## Workflow

### 1. Decide the tax split — the most important rule
- **Place of supply = seller's state (intra-state):** charge **CGST + SGST** (half the GST rate each).
  Example: 18% GST in Maharashtra → 9% CGST + 9% SGST.
- **Place of supply = different state (inter-state):** charge **IGST** (the full rate, one line).
  Example: seller in Maharashtra, buyer in Karnataka, 18% → 18% IGST.
- The buyer's state on the invoice decides this — not where the goods are shipped from alone. If unsure, ask.

### 2. Check the invoice has every mandatory field
- Seller name, address, GSTIN
- Invoice number (sequential, unique for the financial year) and date
- Buyer name, address, GSTIN (B2B) and place of supply
- Item lines: description, HSN/SAC, quantity, taxable value, discount if any
- Tax lines matching step 1 (CGST+SGST **or** IGST — never both on the same line)
- Total in figures **and** in words (Indian numbering: lakh/crore wording is normal)
- Reverse-charge flag if applicable (state it clearly; if unsure, mark `verify before use`)
- Signature / authorised signatory block

### 3. Build the HSN/SAC summary
Group items by HSN/SAC + GST rate and show: total taxable value and tax per group.
This summary is what makes return filing (GSTR-1) easy later — always include it.

### 4. Add payment details (optional but useful)
- UPI ID / UPI QR for the exact invoice amount, bank name + IFSC block if the business uses it.
- Due date and late-payment note if the business has one.

## Invoice template (structure)

```
TAX INVOICE
<Seller Name>                                    Invoice No: <2026-27/001>
<Seller Address, State>                          Date: <DD-MM-YYYY>
GSTIN: <Seller GSTIN>

Bill To:
<Buyer Name>
<Buyer Address, State>          Place of Supply: <State>
GSTIN: <Buyer GSTIN, if B2B>

#  Description        HSN/SAC   Qty   Rate      Taxable Value
1  <Item/Service>     <code>    <n>   <₹>       <₹>

                                   Taxable Total:  <₹>
                                   CGST @<x>%:     <₹>   (intra-state only)
                                   SGST @<x>%:     <₹>   (intra-state only)
                                   IGST @<x>%:     <₹>   (inter-state only)
                                   Grand Total:    <₹>
Amount in words: <Rupees ... Only>

HSN/SAC Summary:
HSN/SAC  Taxable Value   Rate   Tax Amount
<code>   <₹>             <x>%   <₹>

Authorised Signatory: ______________
```

## Rules & common mistakes
- ❌ Charging CGST+SGST on an inter-state sale (most common error) — use IGST.
- ❌ Mixing CGST/SGST and IGST on the same invoice line.
- ❌ Missing place of supply — without it the tax split cannot be justified.
- ❌ Reusing an invoice number in the same financial year.
- ❌ Guessing a GST rate — rates differ by HSN/SAC; if unsure say so and mark `verify before use`.
- ✅ Round the grand total to the nearest rupee and show the round-off line if used.
- ✅ This skill makes a normal tax invoice. It does **not** generate an e-invoice IRN or e-way bill — say this clearly if the user asks.
