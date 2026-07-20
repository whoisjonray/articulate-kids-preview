# Articulate Kids — Pre-Migration SEO Baseline (2026-07-20)

Source: Moz (dashboard PDF + rankings CSV, 2026-02-01 → 2026-07-01) in this folder, plus GSC (whoisjonray@gmail.com).
Purpose: the "before" snapshot. After the staging build flips live, diff against this to prove **zero ranking loss**.

## Top-line (Moz, July 2026)
- **Total visits: 2,368/mo, +50% MoM** (Organic 1,628 · Direct 730). Traffic is UP — do not disrupt.
- Keywords ranked #1–10: **14 of 162 tracked** (competitors: London Speech Therapy 66, Unlocking Language 38, The London Clinic 10).
- Domain Authority: **10** (competitors 30 / 53 / 26). Backlinks: **32** (competitors 1,407 / 190 / 91k). → low authority, so rankings are fragile; migration must be clean, and backlinks/DA are the real growth lever later.
- Moz "search visibility" 1.56% (down MoM) but traffic up 50% — the local pages are carrying real traffic regardless of the composite score.

## The value is concentrated here — PROTECT VERBATIM (same URL + same H-structure)
City/local pages hold nearly all the top rankings. These are non-negotiable to transfer 1:1.

| URL | Best rank | Keyword(s) |
|---|---|---|
| /speech-therapist-chislehurst/ | #1 | speech therapist chislehurst |
| /speech-therapist-petts-wood/ (ranks via /) | #1 | speech therapist petts wood |
| /speech-therapist-sidcup/ | #1 | speech therapist sidcup |
| /speech-therapist-west-wickham/ | #1 | speech therapist west wickham |
| /speech-therapist-bromley/ | #2 | speech therapist bromley |
| /speech-therapist-beckenham/ | #3 | speech therapist beckenham |
| /speech-therapist-bexley/ | #3 | speech therapist bexley |
| /speech-therapist-orpington/ | #3 | speech therapist orpington |
| /speech-therapist-london/ | #3 | eltham, harley street (#9), teenagers, etc. |
| / (homepage) | #1–#8 | speech therapy for kids/children, speech therapist for kids, children's speech therapist |
| /when-should-my-child-start-talking-age-by-age-speech-milestones/ | #13 | should children be talking at 2 years |

Also present in sitemap and to keep: all other /speech-therapist-* city pages (belvedere, bexleyheath, dartford, sidcup, etc.), /conditions-help/*, /ehcp-tribunal-expert/, and the full blog.

## GSC actual traffic (whoisjonray@ · property = https://articulatekids.co.uk/ non-www · last 90d)
Canonical property is **non-www** (www property is empty — 3 clicks). Raw pulls saved: `gsc-nonwww-queries-90d.csv`, `gsc-nonwww-pages-90d.csv`.
- **90-day totals: 3,094 clicks · 281,799 impressions.** Big reach, avg position ~7-9 (mostly page 1 bottom / page 2 — lots of upside from on-page + the migration).

**The real traffic engine is the BLOG, not the city pages.** Moz shows city pages at #1-3 (local dominance, tiny volume). GSC shows the clicks actually come from informational toddler/late-talking articles. Top clicked pages (90d):

| Page | Clicks | Impr | Pos |
|---|---|---|---|
| /18-month-old-not-talking-when-to-worry-vs-when-to-wait/ | **1,076** | 61,994 | 6.9 |
| /late-talking-signs-in-toddlers-red-flags-vs-normal-variation/ | 278 | 34,261 | 5.7 |
| /when-should-my-child-start-talking-age-by-age-speech-milestones/ | 211 | 75,073 | 8.6 |
| / (homepage) | 179 | 6,109 | 17.4 |
| /potty-training-for-neurodivergent-children.../ | 176 | 14,496 | 9.9 |
| /how-diet-affects-your-childs-speech-language-and-attention.../ | 161 | 16,193 | 7.5 |
| /ehcp-tribunal-expert/ | 99 | 1,696 | 7.1 |
| /the-alarming-decline-in-childrens-motor-skills.../ | 99 | 4,456 | 7.7 |
| /courses/the-connected-parent-pathway/lessons/... | 72 | 3,271 | 9.6 |
| /adhd-and-speech-language-therapy-at-articulate-kids/ | 52 | 5,320 | 9.7 |
| /speech-therapist-dartford/ | 52 | 866 | 14.4 |
| /working-memory-and-dyslexia.../ | 47 | 5,933 | 9.5 |

**58 pages earn clicks.** Migration implication: the highest SEO risk is the **blog**, not the local pages. Every blog URL + its content + H-structure must transfer verbatim. This is also why Hulya's "what happens to the articles?" matters — the articles ARE her traffic. (Note: a Connected Parent Pathway *lesson* page earns 72 clicks/mo — before shelving the course to a freebie, 301 that URL so we don't lose it.)

## Migration QA checklist (run on staging before flip)
- [ ] Crawl old site + new staging; diff every URL (no drops), title, H1/H2/H3, meta description, canonical, schema.
- [ ] City pages transferred verbatim (identical rendered text to Googlebot).
- [ ] 301 map for any URL that must change (goal: none).
- [ ] XML sitemap parity + robots.txt + llms.txt (AEO/AI-crawler coverage — a client already found her via Claude).
- [ ] Render as Googlebot + AI crawlers (staging) and confirm content parity.
- [ ] Flip on a low-traffic weekend (target Sat Aug 2); keep old server as instant rollback.
- [ ] Post-flip: submit sitemap in GSC, monitor coverage + rankings daily for 2 weeks; re-pull Moz and diff vs this baseline.
