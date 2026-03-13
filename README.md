# Bonus Scheme vs Profit Sharing Calculator

Interactive calculator comparing employee payouts under a Bonus Scheme vs Profit Sharing model.

## Features

- **4 sliders**: Annual salary, revenue, team size, and profitability
- **Live curve chart**: Continuous payout curves across 0-55% profitability
- **Tier bar chart**: Side-by-side comparison at each 5% step
- **Yellow marker**: Tracks your current profitability setting on both charts
- All amounts in GBP (£)

## Formulas

**Bonus Scheme**: `Bonus % x (Annual Salary / 12)` - where Bonus % is a step function based on profit margin tiers (0% to 220% of one month's salary).

**Profit Sharing**: `(Margin - 10%) x Revenue / 2 / Team Size` - only kicks in above 10% profitability. Excess profit is split 50/50 between company and team, then divided equally.

## Deploy

This is a single static HTML file - no build step required.

```bash
vercel --prod
```

## Tech

- Chart.js 4.4.1
- Vanilla HTML/CSS/JS
- No build tools or dependencies
