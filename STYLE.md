# Manual style

**Law** is `/mnt/d/Bridge/SYSTEM.md`. This folder explains it. If they disagree, SYSTEM wins.

Read these files in **Typora**, **Obsidian**, or a browser. The Grok TUI will show the raw HTML color tags.

---

## Colors

| Kind | Color | When |
|------|--------|------|
| **Announce** | blue `#1565C0` | ACBL announcement (range, transfers, SF 1NT) |
| **Alert** | red `#C62828` | ACBL alert (artificial / unexpected meaning) |
| Natural | black (default) | No announcement, no alert |

**Section headers** for an announceable or alertable call use the same color as the call.

**Example auctions** paint each call that needs an announcement or alert. Pass, natural suits, and to-play bids stay default.

### Copy-paste

Announce:

```html
<span style="color:#1565C0;font-weight:700">1NT</span>
```

Alert:

```html
<span style="color:#C62828;font-weight:700">3♦</span>
```

Header (announce):

```markdown
## <span style="color:#1565C0">1NT opening — announce 11 to 14</span>
```

Header (alert):

```markdown
## <span style="color:#C62828">1♥ / 1♠ – 3♦ — 4-card limit</span>
```

Do not use a third color. Do not mark a bid red “because it is conventional” if ACBL only requires an announcement (transfers, 1NT range, SF 1NT).

---

## Example layout

Every deal uses the same skeleton:

1. **Hands** — NESW, dealer, vulnerability.
2. **Auction table** — colored bids in the table cells.
3. **Why** — one short paragraph: which analog bin, which bucket (no / sure / doubt).
4. **Tell the opponents** — announcement or alert script, or “nothing.”

```markdown
**Dealer South · neither vul**

| | ♠ | ♥ | ♦ | ♣ |
|--|--|--|--|--|
| **S** | AJxxx | Kx | Qxx | xxx |
| **N** | Kxx | Axxx | Kxx | Axx |

| West | North | East | South |
|------|-------|------|-------|
| | | | 1♠ |
| Pass | <span style="color:#C62828;font-weight:700">3♦</span> | Pass | 4♠ |
| Pass | Pass | Pass | |

**Why:** 4-card limit opposite an unlimited 1♠. South has an easy game.

**Tell the opponents:** Alert 3♦ — “four-card limit raise.”
```

---

## Voice

- Matchpoints unless a deal says otherwise.
- Address Jay and Pat. Pat is he/him.
- Treatments are fine. Purely artificial *openings* are not (except strong 2♣).
- Do not invent law in a chapter. If a hole appears, park it and fix SYSTEM.md first.
