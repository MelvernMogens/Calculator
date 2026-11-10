# Sinar Bulian Jaya Calculator

**A one-page calculator for rubber purchase notes: weight × price per kg, minus commission, labour and stamp duty.**

Built for daily use at PT Sinar Bulian Jaya's rubber buying operation, where each purchase is weighed in batches and the payout has fixed deductions. It runs in any browser, phone included, with nothing to install.

**Live:** https://melvernmogens.github.io/Calculator/

## Features

- Add or remove as many weighing rows as you need (**+ Add** / **−**). Each row is `Weight (kg) × Price (Rp/kg)`.
- Running **Subtotal** and **Grand Total** in Rupiah, updated as you type.
- Optional deductions (checkboxes):
  - **Komisi** – 1% of the subtotal
  - **Buruh** – Rp 35 per kg of total weight
  - **Materai** – flat Rp 6,000
- Rounds to the nearest Rp 1,000 the way the business does it: row and grand totals round down unless the last three digits are ≥ 998; commission and labour round up once they pass Rp 2.

## Run locally

It's a single file with no dependencies:

```bash
git clone https://github.com/MelvernMogens/Calculator.git
open Calculator/index.html   # or just double-click it
```

To change the rates, edit the `calculateTotal()` function in the `<script>` block of `index.html`.

## Related

The full purchasing system for the same company lives in [sinar-bulian-jaya](https://github.com/MelvernMogens/sinar-bulian-jaya).

---

Built by [Melvern Mogens](https://github.com/MelvernMogens).
