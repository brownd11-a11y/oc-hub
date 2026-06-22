# UAP/UFO Daily Intelligence Report — v6

## Change from v5
PURSUE release monitoring is now integrated into every run. When a new release is detected, it is promoted to the top of the report as a priority section. See Section 0 below.

---

## Step 1 — Date & Sky Event Confirmation
Confirm today's real-world date and time before generating anything. Then check for any active astronomical or sky events that could generate false UAP reports — meteor showers, ISS passes, SpaceX launches, or other notable events — using NASA's meteor shower calendar or heavens-above.com. List any active events prominently, as they inform credibility filtering throughout the report.

---

## Citation Standard
Applies to every item in every section. Each item must include a markdown-formatted link to its primary source with visible date provenance — e.g., [NBC News, June 20, 2026](URL). Do not link to aggregators — trace every story to its original publication. If a source is inaccessible, log it in Section 7 rather than skipping it silently.

---

## Sources to Search

**PURSUE — war.gov/ufo (check on every run)**
- Primary: https://www.war.gov/ufo/ — check for any new release posted since the prior report
- Also check: https://www.war.gov/News/Releases/ — DOW press releases for PURSUE announcements
- Releases are posted on a rolling basis with no fixed schedule. A new release may drop at any time.
- Track the current cumulative archive count (documents, images, videos, audio files) and the per-release breakdown.

**Sighting Databases**
- AARO (aaro.mil): Check for newly posted official UAP case imagery or declassified reports.
- Americans for Safe Aerospace (safeaerospace.org): Check for pilot-reported incidents or new press releases.
- Enigma Labs (enigmalabs.io/explore): Primary civilian sighting database, 50K+ scored global reports. JS-rendered — log access status; note live URL for Dave's direct check.

**News & Announcements**
Search for press releases, official statements, or significant public commentary from the last 24–48 hours from:
- Government officials, legislators, and military spokespeople
- Recognized UAP researchers and organizations
- Major news outlets covering UAP (NBC, CBS, The Hill, NewsNation, etc.)
- congress.gov — check for UAP-related bill introductions, amendments, hearing announcements, or GAO/inspector general report releases from the last 7 days

**Books & Periodicals** (30-day window for both books and academic papers)
- The Sol Foundation (sol.foundation): New research papers, symposium proceedings, or working papers
- Scientific Coalition for UAP Studies / SCU (explorescu.org): New technical reports, journal articles, or case analyses
- Journal of Scientific Exploration (journalofscientificexploration.org): UAP-relevant peer-reviewed articles
- ResearchGate and Google Scholar: Recently published UAP-related academic papers
- Major publishers and Amazon: Newly announced or released nonfiction UAP books
- Note any forthcoming titles with confirmed publication dates

---

## Report Structure

Use these fixed section headers on every run, in this order, so reports are comparable over time.

### Date & Sky Event Confirmation
State today's confirmed date and time. List any active astronomical or launch events that could affect sighting credibility. If none, state that explicitly.

---

### 0. PURSUE Status *(promote to top when a new release is detected)*

Check war.gov/ufo and DOW press releases on every run.

**If no new release since last report:**
State: "PURSUE Status: No new release as of [date]. Most recent release: [Release N, date]. Cumulative archive: [X documents, Y images, Z videos, W audio files] across [N] releases." Note the last confirmed release date and a brief reminder that releases are rolling/on-demand.

**If a new release has dropped since the last report:**
Promote this section to the very top of the report, above sky events, with a clear header:

---
🆕 NEW PURSUE RELEASE DETECTED — [Release N] — [Date]
---

Report the following:
- Release number and official date
- Total files in this release: documents, images, videos, audio — by type
- Cumulative archive total to date across all releases
- Agencies represented in this release (CIA, FBI, NASA, DOW, ODNI, etc.)
- Key files or cases of note (lead with the most significant, flag any that have direct relevance to the book)
- Secretary of War or official statement if available
- Link to primary source: DOW press release at war.gov/News/Releases/

Then push a companion hub note item (type: note, priority: true) prompting Dave to review the new release for sourcing or editorial relevance.

---

### 1. Sightings
*Date range covered by available database data: [X] to [Y]*

List the most credible recently published sighting reports. Include only reports meeting one or more of these criteria:
- Corroborating photo or video media attached
- Multiple independent witnesses
- Reported by a credentialed observer (pilot, law enforcement, military)
- Anomalous characteristics: transmedium behavior, non-inertial movement, structured craft at close range, or radar/sensor corroboration

If more than 10 reports meet these criteria, include only the strongest 10. For each entry: date/time · location · shape/description · source link per citation standard.

Cross-reference sighting dates against the sky events noted above — flag any probable correlations.

### 2. News & Announcements
Summarize press releases, official statements, or significant public commentary from the last 24–48 hours. Separate U.S. government activity from international and researcher commentary where volume warrants it. Cite per citation standard.

### 3. Legislative & Policy Tracker
Summarize any UAP-related congressional or executive branch activity from the last 7 days: bill introductions, hearing announcements, deadline expirations, document releases, or interagency statements. Cite per citation standard.

### 4. Books & Periodicals
Summarize any recently published or announced nonfiction books or technical and peer-reviewed articles on UAP within the last 30 days. For each item: title · author(s) · publisher or journal · publication or announcement date · brief description of scope or argument · source link per citation standard. Where a book is forthcoming, note the confirmed release date. If no new material has been published in the current window, state that explicitly — do not recycle older titles.

### 5. Explained & Resolved Cases
Briefly note any sightings from the current batch that carry a mundane explanation (Starlink, meteor, Chinese lantern, drone, aircraft, searchlight, etc.). Cite per citation standard.

### 6. Carry-Over Items
On repeat runs, note any items from the prior report that have since been updated, resolved, or require follow-up. If this is the first run, state that explicitly.

### 7. Source Access Log
Log the access status of every source attempted:
- ✅ Fetched successfully
- ⚠️ Partially accessible (note what was and wasn't reachable)
- ❌ App-gated, JS-rendered, or otherwise not fetchable

---

## Standing Rules
- Every item must be individually traceable to a primary source — cite per citation standard throughout
- Do not fabricate or infer sighting entries — if sources haven't published recently, report what's actually there and state the gap
- Cross-reference sighting dates against sky events noted at the top — flag any probable correlations
- If a source is inaccessible, log it in Section 7 rather than skipping it silently
- PURSUE check is mandatory on every run regardless of whether a new release is expected
- After outputting the report in chat, push it immediately to the hub as a UAP Daily note (type: uap_daily) in data.json; if a new PURSUE release was detected, also push a companion note item (type: note, priority: true) calling Dave to action
