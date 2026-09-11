# Pendu Arena — Prototypes

Clickable HTML prototypes for Pendu's esports tournament flow.

**Live:** https://vay-dev.github.io/pendu-prototypes/

## Tournament lifecycle prototype

`index.html` — a self-contained prototype of the full tournament lifecycle,
entered from the Hub tab:

| Step | Screen |
|---|---|
| 0 | Hub — tournament discovery (entry point) |
| 1 | Tournament lobby — prize pool, slots, organizer rules |
| 2 | Squad registration — roster, K/D stats, escrow payment |
| 3 | Match lobby & check-in — countdown, room credentials |
| 4 | Live stream — video, floating chat, spectator gifting |
| 5 | Bracket & result submission — knockout tree, OCR evidence |
| 6 | Victory & payout — podium, MVP, escrow split |

### Notes

- **Design system:** Stitch "Apex Esports Dark Engine" (Outfit + JetBrains Mono,
  deep OLED surfaces, tactical HUD glassmorphism).
- **Navigation** mirrors the real app — bottom nav from `main_app_shell.dart`
  on mobile, and the `pendu-web` sidebar at ≥1024px.
- **Live indicator** is the Pendu 3-bar waveform ported from
  `lib/presentation/widgets/common/live_waveform.dart` (400/520/360ms).
- Sound is synthesized with the Web Audio API — no audio assets.
- Keyboard: `0`–`6` jump between steps, `←`/`→` step through, `f` toggles
  fullscreen on the stream, `Esc` closes sheets.

Prototype only — not production code.
