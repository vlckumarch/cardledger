# CardLedger — Credit Card Bill Tracker

A lightweight, responsive credit-card bill tracker that can be hosted for free on GitHub Pages.

## Features

- Add one monthly statement record per card, including statement month, due date, amount spent, amount to pay, paid/unpaid status, paid date, and notes.
- Dashboard totals for all-time spending, year-to-date (YTD) spending, this month's payable amount, and unpaid bills.
- Monthly spending chart and year-by-year totals for current and previous years.
- Filter bills by year, card, and payment status; search by card or notes.
- Edit and delete records.
- Export records as CSV and back up/restore all data as JSON.
- Responsive layout for desktop and mobile.

## Deploy to GitHub Pages

1. Create a new GitHub repository, for example `cardledger`.
2. Upload `index.html`, `README.md`, and `.nojekyll` to the repository root.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main` and folder `/ (root)`, then click **Save**.
6. Wait for the Pages deployment to finish. Your app URL will be shown in the Pages settings.

No build step, package manager, or server is required.

## Data and privacy

This is a static, client-side app. Entries are stored in the current browser's `localStorage`; they are not synced between browsers or devices and are not uploaded to GitHub. Anyone with access to the same browser profile may be able to view them. Export a JSON backup periodically. Clearing site data/browser storage can erase records.

## Calculation definitions

- **Amount spent** is summed by statement month to calculate monthly, YTD, annual, and all-time spending.
- **Amount to pay** is used for this month's payable total and the unpaid/overdue total.
- YTD means January through the current calendar month, using the current local date.
- Previous-year totals are calendar-year totals based on the statement month.

## Suggested next improvements

- Optional password-protected account and cloud sync (requires a backend).
- Payment reminders and recurring bill templates.
- Import existing statements from CSV.
