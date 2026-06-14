# iOS App — Options and Recommendation

## Context
The hub (hub.over-classified.com) is a browser-based HTML5 app. Most of its logic 
is portable; the UI layer needs rethinking for native iOS patterns.

---

## What carries over without rewrite
- Data model (data.json — items, road, outreach, refs)
- GitHub sync pattern (fetch on load, push on change)
- All business logic: filtering, threading, dialogue, roadmap phase/step/gate relationships
- Pure JavaScript — runs identically in a WKWebView

## What needs rethinking for native iOS
- Fixed-position overlays → navigation stack + bottom sheets
- Hover states → tap / long-press
- Right-click context menus → swipe actions (delete/defer/done)
- Keyboard shortcuts → toolbar buttons or gesture shortcuts
- Gantt chart → UIScrollView with custom drawn layer (most work)

---

## Three paths — rough order of effort

### 1. Progressive Web App (PWA) — 2–3 hours
Add a web manifest and service worker to the existing hub.
- Installable from Safari → home screen icon
- Full-screen mode (no browser chrome)
- Offline capability via cache
- Looks/feels like a web app, not native — acceptable for single-user tool
- No App Store required

### 2. WKWebView wrapper — 2–3 days
Thin Swift app that loads the hub in a full-screen web view.
- Adds push notification support
- Optionally adds a share extension
- App Store eligible but Apple scrutinizes web-wrapper apps heavily
- May not pass App Store review

### 3. Native SwiftUI — 3–4 weeks
Full rewrite of the UI layer, keeping data model and GitHub sync.
- Genuinely excellent on iPad (Gantt + Notes list map well to SwiftUI primitives)
- Swipe actions, share sheets, proper navigation stack
- Data model is already clean enough to hand off to a SwiftUI developer
- Most effort; best result

---

## Recommendation
Start with PWA. Closes 80% of the gap for 5% of the effort. Live with it. 
If unsatisfying, the data model is ready for a native handoff.

## To implement PWA
Claude adds two files to the oc-hub repo:
1. manifest.json — app name, icon, display:standalone, theme color
2. sw.js — service worker caching the hub shell

Then adds two <link> tags to index.html pointing to them.
Total push: ~30 minutes.
