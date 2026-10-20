# Last Chair

The spreadsheet I kept for fifteen years, turned into an app.

A private planner for financial independence. It puts everything a household owns on one page and answers one question: what year does work become optional? I designed, built and launched it in October 2026 at https://lastchair.app.

## Why I built it

For more than fifteen years I kept a spreadsheet to answer that question. It tracked my holdings, what each fund cost in fees, and the year the numbers said I could stop. I was always tweaking it.

The habit came from the Bogleheads forum and a few of the Bogleheads books: low-cost index funds, a simple mix, and staying the course. Over the years the sheet turned into spreadsheet chaos: balances typed by hand, formulas that broke when a row moved, coins Google Sheets couldn’t price, and a rebalance that said “buy more international” but never which fund, in which account. I wanted it to run itself, and I thought it could help other people who run their own money the same way.

## What it does

You enter tickers and share counts, coins, or a plain balance for anything without a price, plus a home and its mortgage. Prices and fund fees look themselves up. From there Last Chair shows net worth, how the mix compares with your targets, the year work becomes optional and whether you could already stop saving, and the trades that put the mix back on target: which fund, in which account, with the tax of each.

## Private by design

There are no bank or brokerage logins, ever, and no aggregator in the middle. Accounts are labels, not account numbers. The household is one document, encrypted in the browser before it is saved: AES-256-GCM under a key derived from your passphrase with Argon2id, on your device. Twenty-four recovery words are the way back in, and a passkey can unlock it too. The server stores ciphertext it can’t read, every calculation runs in the browser, and price lookups carry only public ticker symbols.

That rule shaped the whole build. It is also why the public pages run on an invented household, never my own.

## Tested against history

A single average return hides the bad decades. Last Chair replays the plan as if you’d started in each year of US markets since 1928, through what actually came next, 1929, 1966 and 2008 included, and through a Monte Carlo of two thousand markets resampled from that record. The answer is how many of those histories the money lasts in. The annual returns are Aswath Damodaran’s, credited in the app.

## The Fee Finder

The one piece anyone can use without an account. Enter what you hold and roughly how much, and it shows what the fees cost a year, by the age you’d like to stop, and in months of work, against low-cost twins of the same funds. Expense ratios come from SEC filings. Try it at https://lastchair.app/fees.

## Charts and math

The charts are mine, hand-built in SVG with D3: a century of markets where each start year is a line that folds into a bar, the range of outcomes, the holdings as an icicle, the lifetime cost of fees. The Monte Carlo runs in a background worker in the browser and draws each run as it lands, so none of the math needs a server.

## Links

- Last Chair: https://lastchair.app
- Fee Finder (free, no sign-up): https://lastchair.app/fees
- Why Last Chair: https://lastchair.app/why
- How the encryption works: https://lastchair.app/security

Last Chair provides planning tools, not investment advice.
