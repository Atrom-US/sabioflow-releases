<div align="center">

<img src="assets/icon.png" width="120" alt="SabioFlow icon" />

# SabioFlow

**Personal finance for Mac that lives on your Mac.**<br />
No account. No cloud. No tracking. Just your money, in a file you own.

[**Download for Mac**](https://github.com/Atrom-US/sabioflow-releases/releases/latest) &nbsp;·&nbsp; [What's new](https://github.com/Atrom-US/sabioflow-releases/releases) &nbsp;·&nbsp; [License](LICENSE) &nbsp;·&nbsp; [atrom.us](https://atrom.us)

![Platform](https://img.shields.io/badge/macOS-13%2B-black?logo=apple&logoColor=white)
![Apple Silicon](https://img.shields.io/badge/Apple%20Silicon-arm64-7c3aed)
![Latest release](https://img.shields.io/github/v/release/Atrom-US/sabioflow-releases?color=7c3aed&label=latest)

<br />

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/dashboard-dark.png" />
  <img src="assets/dashboard-light.png" alt="The SabioFlow dashboard: net worth, income, expenses, savings, cash flow and spending by category" width="900" />
</picture>

</div>

<br />

## Why SabioFlow

Most money apps want your login, your bank credentials and a monthly fee, and then keep your data on their servers. SabioFlow does the opposite.

- 🔒 **Your data stays with you.** Everything lives in a single `.sabioflow` file on your Mac. Back it up, move it, or open it on another Mac like any other document.
- 🔑 **Optional password protection.** Encrypt your file with SQLCipher 4 (AES‑256) and keep the password in your Mac's Keychain.
- 🚫 **No telemetry. No ads. No account.** The app has no analytics and never uploads your data.
- ⚡ **Built to be fast.** A native Mac app (Tauri 2 + Rust) with a register that stays smooth even with years of history.
- ♿ **Accessible by design.** Full keyboard control, light and dark modes, checked against WCAG 2.2 AA.

## What you can do

<table>
<tr>
<td width="50%" valign="top">

### 📊 A dashboard that answers “how am I doing?”
Net worth, income, expenses and savings at a glance, with cash flow, spending by category, trends and a map of where your money comes from and where it goes.

</td>
<td width="50%" valign="top">

### 📒 A register that keeps up with you
Add transactions in a fast inline row (`⌘N`), type a calculation like `(4*2)+1/2` in any amount, split across categories, tag with suggestions, link transfers, edit many at once with `⌘E`, and undo with `⌘Z`.

</td>
</tr>
<tr>
<td valign="top">

### 🏦 Connect your accounts, privately
Sync your banks through [SimpleFIN Bridge](https://www.simplefin.org/) and your brokerages, read-only, through [SnapTrade](https://snaptrade.com/). Credentials are stored only in your Mac's Keychain, never in your file. SabioFlow never places, changes or cancels an order.

</td>
<td valign="top">

### 📈 Investments in the same place
See each investment account's total value, how much is invested and how much is cash, plus a value-over-time chart, next to your everyday accounts and in your net worth.

</td>
</tr>
<tr>
<td valign="top">

### 📥 Bring your history with you
Import CSV, OFX, QFX, QIF, Quicken ZIP and `.quicken` files, or just drag a file onto an account. Re-importing never duplicates what you already have, and every import is a batch you can review and undo.

</td>
<td valign="top">

### 🧠 Smart categorization
Rules and suggestions learn from how you categorize. The **Review** inbox catches new, uncategorized and possible transfer transactions, and links a refund to the purchase it corrects so your spending stays right.

</td>
</tr>
<tr>
<td valign="top">

### 🗓️ Budgets and reports you can act on
A monthly budget that shows what is left in every category, scheduled transactions, and spending, income, cash flow and net worth reports. Save the ones you use and export them to CSV.

</td>
<td valign="top">

### 🏢 Personal and business, side by side
Keep business accounts separate, assign a business expense paid with a personal card, and track money you lend or owe to people.

</td>
</tr>
</table>

Also included: tags, attachments, reconciliation, multiple currencies (USD, COP, MXN and EUR with automatic exchange rates or your own), automatic and manual backups, global search (`⌘F`) and an interface in **English and Spanish**.

## A closer look

<table>
<tr>
<td width="50%">
<img src="assets/register-dark.png" alt="The transaction register in dark mode, with an account summary, categories and a running balance" />
<p align="center"><sub><b>Register</b> — fast, keyboard-friendly and always balanced</sub></p>
</td>
<td width="50%">
<img src="assets/accounts-light.png" alt="One list of accounts grouped by bank, with SnapTrade and manual accounts" />
<p align="center"><sub><b>Accounts</b> — one list, grouped by bank</sub></p>
</td>
</tr>
<tr>
<td>
<img src="assets/budget-dark.png" alt="The monthly budget in dark mode showing what is left in each category" />
<p align="center"><sub><b>Budget</b> — see what is left in every category</sub></p>
</td>
<td>
<img src="assets/investments-dark.png" alt="An investment account with its total value, invested amount, cash and value chart" />
<p align="center"><sub><b>Investments</b> — value and history, read-only</sub></p>
</td>
</tr>
<tr>
<td>
<img src="assets/reports-light.png" alt="The spending report with a monthly chart and a breakdown by category" />
<p align="center"><sub><b>Reports</b> — understand your spending in seconds</sub></p>
</td>
<td>
<img src="assets/review-light.png" alt="The Review inbox with transactions waiting for a category" />
<p align="center"><sub><b>Review</b> — nothing slips through uncategorized</sub></p>
</td>
</tr>
</table>

> All screenshots use made-up sample data.

## Download and install

1. Go to the [**latest release**](https://github.com/Atrom-US/sabioflow-releases/releases/latest) and download `SabioFlow_<version>_aarch64.dmg`.
2. Open the `.dmg` and drag **SabioFlow** to **Applications**.
3. Open SabioFlow and create a new document, or double‑click an existing `.sabioflow` file.

**Requirements:** a Mac with Apple Silicon (M1 or later) running macOS 13 Ventura or newer. Intel Macs are not supported yet.

### First launch

SabioFlow is not yet notarized by Apple, so macOS asks for confirmation the first time you open it. You only need to do this once:

- **Right‑click** (or `⌃`‑click) **SabioFlow** in Applications, choose **Open**, then click **Open** again.
- If macOS says the app is "damaged", run this in Terminal and open it again:

  ```bash
  xattr -dr com.apple.quarantine /Applications/SabioFlow.app
  ```

## Updates

SabioFlow checks for new versions at most once a day (you can turn this off in **Settings › General**, or check any time from **SabioFlow › Check for Updates…**). It always shows you what changed and **never installs anything on its own**.

Before installing, the app verifies the update's cryptographic signature and makes a backup copy of your open document. The only thing the check downloads is a small public file with the latest version number; nothing about you or your data is sent.

## Privacy

- No analytics, no crash reporting, no accounts.
- Your document never leaves your Mac unless you move it yourself.
- The app only connects to the internet to:
  - fetch exchange rates (it sends only currency codes and dates),
  - sync your bank through SimpleFIN, **if you choose to connect it**,
  - read your brokerage accounts (read-only) through SnapTrade, **if you choose to connect it**, and
  - check for updates.

## License

SabioFlow is proprietary software, **not open source**. This repository contains only release builds and documentation. See [LICENSE](LICENSE) for the terms that apply to using the app.

<br />

<div align="center">
<sub>Made by <a href="https://atrom.us">Atrom</a> · © 2026 zjubiz. All rights reserved.</sub>
</div>
