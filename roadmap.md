# Grapher Roadmap

## From Apps.pdf (imported 2026-07-12)
- [ ] Ship iOS: blocked — no ASC app record for com.nulljosh.grapher; register app first (asc-app-create-ui skill, browser automation, confirm first), then `asc workflow run ship-ios`

## WKWebView shell (reviewed 2026-07-22)
Not a gap — `CLAUDE.md` documents this as intentional ("app has no native API needs"). Unlike Books, this was a deliberate choice, not an oversight. Revisit only if grapher ever needs a real native API (e.g. share sheet, widgets) that the web shell can't provide. If it's ever ported anyway, the blocker is replacing `mathjs` expression parsing/eval with a Swift equivalent — everything else (canvas plotting, equation list UI) maps cleanly to SwiftUI `Canvas`.
