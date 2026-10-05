# Trading Work Log

A simple, single-page work log for tracking daily tasks, buy/sell trades, proof photos and withdrawal proofs. Works on desktop and mobile, with light and dark themes.

**Live site:** https://devarajakasi-eng.github.io/work-log-/

## Features

- **Tasks** – start/end timer per task, edit times, mark done, total hours per day
- **Buy / Sell** – log trades with profit/loss, currency per day, attach photos to each trade
- **Proof** – upload and view daily proof photos
- **Withdraw Proof** – log withdrawals by attaching proof photos
- **Daily Report** – pick a date range, preview the report, download as PDF or print
- **PIN lock** – the log asks for a PIN before editing; a wrong PIN opens a read-only view
- **Auto cleanup** – entries older than 30 days are removed automatically

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole app (HTML, CSS and JavaScript in one file) |
| `README.md` | This file |

## Deploy on GitHub Pages

1. Upload `index.html` and `README.md` to the root of the repository.
2. Open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select branch `main` and folder `/ (root)`, then click **Save**.
5. After a minute or two the site is live at the link above.

## Notes

- All data is stored in the browser's local storage on each device. Phone and computer do not sync.
- Clearing browser data removes the log. Download PDF reports to keep a copy.
- The PIN check runs in the page itself, so it is a casual lock and not real security. Do not store sensitive information.
- PDF export uses [jsPDF](https://github.com/parallax/jsPDF) loaded from cdnjs, so an internet connection is needed for PDF download.
