# Troy Student Managed Portfolio Management System

This updated prototype combines trade workflow, live holdings, performance tracking, benchmark comparisons, macro/market dashboard scaffolding, and permanent trade-history export in one browser-based application.

## What was added

- **Live Portfolio** page with Excel/CSV holdings import
- Holdings table modeled on brokerage-style portfolio views
- Portfolio value, cost, gain/loss, holdings count, cash, sector filter, current weight, and target weight
- **Daily Portfolio Snapshot** storage for building a historical performance series
- **Performance & Benchmarks** page
  - Total Troy SMP vs. **SPY**
  - Sector comparison using ETF proxies: XLC, XLY, XLP, XLE, XLF, XLV, XLI, XLK, XLB, XLRE, XLU
  - Active-return KPI
  - View and period dropdowns
  - Benchmark Excel/CSV import and downloadable CSV template
- **Macro & Market Dashboard** scaffold for major indicators
- Revised trade workflow: Sector Lead → Compliance Officer → Portfolio Director → Instructor → Head Trader executes
- Head Trader no longer serves as an approval gate
- Expanded execution record with shares, price, order type, timestamp, and optional Investopedia reference
- Trade History CSV export
- Full-system JSON backup download

## Important prototype limitation

This version still stores data in the browser's **localStorage**. If Student A uses the file on one computer and Student B uses it on another, they will not see the same data.

For real shared multi-user use, the next phase should connect the application to a shared database (for example, Supabase/PostgreSQL or a Troy-approved Microsoft solution) and publish the website at a normal `https://` address.

## Files

- `index.html` — complete application
- `README.md` — this guide

## Suggested folder in Teams

`Trade Management > Shared > Trade Management System`

Store the current release and backups there. The Teams folder is document storage; it does not itself turn the HTML file into a shared live web application.
