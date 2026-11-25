# HeadsUp — feed-first frontend prototype

Created from five captured HeadsUp page ZIPs supplied November 2026. This is **not the original Next.js project**, and is not connected to the live backend. It is an independent, responsive static HTML/CSS/JS frontend for client review and developer handoff.

## Pages
- `index.html` — homepage feed, statistics, local gems, community content
- `pages/discover.html` — local places and searchable cards
- `pages/events.html` — captured sample events, searchable cards
- `pages/businesses.html` — Local Gems and business participation
- `pages/about.html` — community, check-ins, rewards and responsibilities
- `pages/favourites.html` — Your Space signed-out state
- `pages/login.html`, `pages/register.html` — phone sign-in UI (no authentication yet)
- `pages/contact.html` — contact form opens email app (not backend-connected)

## Scope and caveats
Captured material represents saved HTML pages, not editable source/API contracts. Event content reflects the captured site dated 25 November 2026; **do not use these events as live listings**. Listing detail links point to the original headsup.community pages. The current source's logo and other proprietary image assets were not included as editable source references in a usable format; the prototype uses a simple typographic HeadsUp placeholder and abstract card artwork. Do not deploy over the production Next.js app. Existing backend operations, event management, saved items, user registration, live feed, business management, and payments need backend developer integration. The PWA manifest is for a presentation shell; offline caching and install icons are not yet implemented.

## Review
Open with a local static server (for example VS Code Live Server). Edit design tokens in `assets/css/styles.css` and data in `assets/js/data.js` (the sample HTML cards are currently embedded in the pages). Connect actual API before production. Confirm client-provided brand fonts/logo. This prototype uses temporary Space Grotesk and DM Sans fallbacks.


## Mobile icon hotfix
Replaced Unicode/emoji navigation and card icons with Font Awesome 6.7.2 (CDN). Fixed the giant iOS-rendered hero emoji by replacing it with a CSS ring. Updated responsive text sizing. Requires internet to load the icon font.
