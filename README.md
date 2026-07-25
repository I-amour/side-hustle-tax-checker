# side-hustle-tax-checker

**Live: https://i-amour.github.io/side-hustle-tax-checker/**

A free checker for UK side hustlers — Vinted, eBay, Etsy, deliveries, freelancing — that answers the question everyone's too scared to google properly: *do I actually owe HMRC anything?*

Type in what you've earned and spent this tax year, and it stamps a verdict (literally — there's a rubber stamp) telling you whether you need to register for Self Assessment and roughly what to set aside.

## Why

Platforms now report UK sellers' earnings straight to HMRC, and millions of people — including me and most of my flat — suddenly needed to know where they stood. The gov.uk pages technically contain the answer. Nobody finishes reading them.

So I built the thirty-second version.

## What it handles

- The **£1,000 trading allowance** — under it, you're fine; the checker tells you how close you are
- The **"I'm just selling my own old stuff" case** — usually no tax at all, and the tool says so instead of scaring you
- **Best deduction logic** — flat £1,000 allowance vs your real costs, whichever saves more
- **2026/27 rates** — income tax bands and Class 4 NI, including how a day-job salary changes the band your side profit lands in
- **Deadlines** — when to register, when to file, what the fine is if you don't

## How it's built

One HTML file. Vanilla JS, no framework, no backend, no analytics, no cookies — nothing you type leaves your device. The design is an old ledger book: ruled paper, red margin lines, and a verdict stamp, because every finance tool on earth is a blue dashboard and I refuse.

Fun fact: the launch build shipped completely broken because I named a variable `£`, which JavaScript does not allow. A currency-themed bug in a currency-themed app. I've left the fix in the commit history as a monument.

## Run it locally

Clone, open `index.html`. That's it. That's the stack.

## Honest limits

This is a record-keeping helper, not tax advice. It keeps things simple on purpose — no student loans, Scottish bands, or the £100k allowance taper. The official checker lives at [gov.uk](https://www.gov.uk/check-additional-income-tax).

## The year-round version

If the checker says you owe tax, the annoying part is keeping records for the next twelve months. I made a [bookkeeping spreadsheet](https://payhip.com/b/TV64S) that does that — tracks income, expenses and mileage, watches the £1,000 line, and estimates what to set aside, all in pure Excel formulas.

---

Built by [Simi Olusola](https://github.com/I-amour) — CS @ Loughborough, class of 2027.
Found a bug or a tax rule I got wrong? Open an issue. I'd rather fix it than be confidently wrong on the internet.
