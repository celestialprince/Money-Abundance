# 💸 Money Abundance — 30 Days Mind Hack

> *"When you hit Day 18 and have to find exactly $18,000 worth of new, exciting things to buy, you realise how deep your scarcity mindset goes."*

A completely private, offline-capable web app for playing **The Prosperity Game** — a psychology exercise designed to dismantle scarcity thinking by forcing your brain to get comfortable spending large amounts of money, every single day.

---

## 🧠 What Is The Prosperity Game?

The Prosperity Game is a mindset exercise that went viral on Threads. The mechanics are deceptively simple:

- **Day 1:** Mentally spend exactly $1,000 CAD
- **Day 2:** Mentally spend exactly $2,000 CAD
- **Day 3:** $3,000 CAD… and so on
- **Day 30:** You have to figure out how to spend $30,000 in a single day

Over the full 30 days, you simulate spending a total of **$465,000 CAD**.

**The catch?** You have to *actually spend it* in your imagination — no high-yield savings, no index funds, and you cannot repeat purchases. You can't just buy 15 MacBooks on Day 15 to clear your balance. You must research and imagine a real, evolving lifestyle every single day.

That's where the mindset shift happens. When you're stuck trying to find $18,000 worth of genuinely new things to buy, you start to realise how deeply programmed your brain is to *not* want things.

---

## 🎮 How to Play

1. **Open Day 1.** You have an allowance of $1,000 CAD. Enter what you'd "buy" (e.g. *Spa day* — $400, *Designer sneakers* — $600) and hit **+ Add**.
2. **Aim for $0.** The balance badge at the bottom changes colour to signal your status:
   - 🟡 **Yellow** — you still have money left to spend
   - 🟢 **Green** — perfectly balanced at exactly $0 (the goal!)
   - 🟠 **Orange** — you've overspent your allowance
3. **Move through the 30 days.** The coloured dot on each tab tells you its status at a glance. Work through all 30 days until every dot is green.
4. **Check your progress** on the **Σ Summary** tab to see your total allowance, total spent, and net balance across all days.
5. **Explore your patterns** on the **✦ Insights** tab — search entries, view a daily spending chart, and see a breakdown by spending category.

If you zero out all 30 days, you will have successfully simulated spending **$465,000 CAD** in one month. 🎉

---

## ✨ Features

### Core
- **30 day tabs** — one per day, each with its own growing allowance
- **Colour-coded balance badge** — yellow (remaining) / green (zero) / orange (overspent)
- **Tab status dots** — see every day's status without opening it
- **Spending categories** — tag each entry: Food, Transport, Shopping, Entertainment, Health, Bills, Other

### Editing
- **Inline edit** — tap the ✎ pencil icon to edit any entry's description, amount, or category without losing your place
- **Delete entries** — tap × to remove a line item
- **Clear Day** — wipe all entries for a single day (with confirmation)
- **Clear All** — nuclear reset of all 30 days (with confirmation)

### Undo
- **Every destructive action is undoable** — deleting an entry, clearing a day, clearing all data, and even imports all push a snapshot to the undo history
- **5-second undo toast** — a blue notification bar appears after any delete or clear action with a one-tap **Undo** button
- Up to 50 undo snapshots are kept in memory per session

### Import / Export
- **Export** — on mobile, opens the native share sheet (AirDrop, iMessage, etc.); on desktop, downloads a `.json` file
- **Import** — pick a previously exported `.json` file to restore your data; current data is saved to undo history before overwriting
- Export format is human-readable JSON with a version field and timestamp

### Insights Tab
- **🔍 Search** — search descriptions and categories across all 30 days; tap any result to jump to that day
- **📊 Spending chart** — scrollable SVG bar chart showing daily allowance vs actual spending for all 30 days; overspent days are highlighted in orange
- **🏷️ Category breakdown** — horizontal bar chart showing your total spending split by category with percentages

### Onboarding
- **First-visit welcome popup** — explains the rules and goal of The Prosperity Game; only appears once, never again after dismissed
- **? Help button** in the header re-opens the welcome popup at any time

---

## 🔒 Privacy & Data

This app is **100% serverless and offline-capable**. There is no backend, no database, no accounts, no analytics, and no network requests after the fonts load.

- All entries are saved to your **device's local browser storage** (`localStorage`)
- Nobody else can see your data — not even the developer
- **Important:** Clearing your browser cache will wipe your data. Use **Export** regularly to keep a backup

---

## 💾 Export File Format

```json
{
  "version": 2,
  "exported": "2026-04-26T10:30:00.000Z",
  "entries": {
    "1": [
      { "id": 1714000000001, "description": "Spa day", "amount": 700, "category": "Health" },
      { "id": 1714000000002, "description": "Designer sneakers", "amount": 300, "category": "Shopping" }
    ],
    "2": [ ... ]
  }
}
```

---

## 📱 Mobile Installation

The app is a single `.html` file. No install required — just open it in a browser.

**iPhone (Safari):**
1. Open the file in Safari
2. Tap the Share button → **Add to Home Screen**
3. It now appears as an app icon and runs full-screen

**Android (Chrome):**
1. Open the file in Chrome
2. Tap the 3-dot menu → **Add to Home Screen**

---

## 🛠️ Tech Stack

- Pure **HTML5 / CSS3 / Vanilla JavaScript** — zero dependencies, zero frameworks
- **SVG** for the spending chart (no charting library needed)
- **localStorage** for persistence
- **Web Share API** for native mobile export (falls back to file download on desktop)
- **Google Fonts** (Playfair Display, Sora, Space Grotesk) — loaded once, cached by browser

Single file. No build step. No npm. Just open and play.

---

## 🙏 Credit

Inspired by the *The Prosperity Game* and the concept of abundance mindset training.
