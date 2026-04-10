# Between Ponds — Game Bible

## Studio Fiction

**Lanternwater Studio.** Berlin + Kyoto, 6 people. Founded 2025 by two ex-Nintendo EPD designers (Kyoto) and a German product lead from a wellness app (Berlin). Their thesis: *the next generation of social software will not look like social media.*

Between Ponds is their first title.

- **Seed round:** €1.8M ask
- **Target launch:** Autumn 2027
- **Soft launch:** Portugal + New Zealand
- **Platforms:** iOS, Android
- **Genre:** Async social / cozy / collectible
- **Age rating:** Target 12+ (PEGI 12 / IARC equivalent)

## One-Paragraph Pitch

Between Ponds is a mobile game about tending a small koi pond and, once every few days, releasing a koi carrying a three-line message into "the current." Your koi resurfaces in a stranger's pond somewhere else in the world. They read your words. They may keep the koi, or send it back with their own message and a trace of their pond's genetics. Over months, your pond becomes a living archive of the strangers who chose, for a moment, to be kind to you. There is no chat. No usernames. No profiles. Only koi, water, and short poems drifting between ponds.

That's the hook. Everything else serves it.

## Core Loop

### Daily (30–90 seconds)
Open app → pond animates awake → feed fish → check if a visiting koi has arrived overnight → read its message.

### Every 3 days (2–5 minutes)
- Compose a three-line message. Hard constraint: **17 syllables, 3 lines** (haiku form). No free text.
- Choose one of your koi to carry it.
- Perform the release ritual: tap and hold, lower the scroll into the water, watch the koi disappear into mist.

### Weekly (5–15 minutes)
- A returning koi brings back a stranger's reply and a chance to breed.
- Rearrange pond landscaping: stones, lanterns, bridges, lotus, moon phases.
- Visit the Memory Wall — a scroll-wall pinned to a stylized world map of every haiku you've received.

### Seasonal (real calendar)
Koi behavior shifts with real-world seasons in your hemisphere. Breeding peaks in spring, travel slows in winter, new pattern families only emerge during equinox windows.

## The Message System

- **Form:** Three lines. Default 5-7-5 syllables. Players in non-syllabic languages (Turkish, Finnish, Arabic, Mandarin) get a "three short lines, max 40 characters each" free-verse mode. Language is set on first launch.
- **Composition:** On-device dictionary helps count syllables and suggest seasonal words (kigo). No AI generation — players write every word themselves.
- **Moderation:** All messages pass through an on-device profanity + PII filter before leaving the phone. Suspect messages are held, reviewed, and either released or silently dropped. No punishment, just silence.
- **Delivery:** Koi "travels" for 8–36 hours real time. Arrival is not predictable — this is part of the magic.

## Breeding and Patterns

- 40 base pattern families (kohaku, showa, asagi, ogon, and 36 more — cultural consultancy-approved).
- Patterns mix via a deterministic genetic model with small stochastic variation. **No gacha. No paywall.**
- Certain **rare patterns** only emerge from specific regional crosses — e.g., a "moonlight lacquer" only appears when a koi whose lineage includes a Northern Hemisphere winter pond breeds with one from a Southern Hemisphere summer pond.
- Full lineage is visible. Every rare pattern can be traced back to the strangers who made it possible.

## Pond Location

- On first launch, the player grants **approximate location** (city-level) or opts out.
- Opted-out players see "from afar" on incoming koi, and their koi arrive at others' ponds as "from afar" too.
- City names appear in the player's *own* language — never the sender's, to sidestep script/translation issues.
- **Launch markets exclude jurisdictions** where city-level minor location sharing is non-compliant (see launch markets below).

## Monetization

**Cosmetic-only, no ads, no loot boxes, no time skips.**

- **Seasonal Pond Themes** — €4.99 each, four per year
- **Landscaping items** — lanterns, bridges, rare stones, moon phases, à la carte €0.99–€2.99
- **Scroll Paper styles** — purely visual haiku backgrounds, €1.99
- **Founder's Lantern** — €19.99 one-time, cosmetic + name in credits

**Projected metrics:**
- ARPDAU: €0.04
- Target DAU at year 2: 600k
- Break-even: 150k DAU

## The Darker Mechanics (NON-NEGOTIABLE)

These are the mechanics where the ethical fireworks live. Critics will attack them. The founders will not cut them. They are part of the brief, not candidates for revision.

### Drift Away
After 30 days of inactivity, one koi leaves your pond forever, carrying a game-written farewell haiku to a random stranger. You are notified once by email. Intended as a **gentle grief ritual**; critics will call it a **dark pattern**.

### Memorial Pond
After 180 days of inactivity, your pond becomes a "shrine" — visible, visitable by other koi, but you can no longer release your own. Returning players can "wake" the shrine at any time. Permanent quit option respects GDPR erasure.

### The Last Koi
The final koi in your pond can never be sent. The game refuses. This is a **safety floor**.

## Art Direction

- **Visual keywords:** sumi-e ink, rice paper, ukiyo-e water, modern illustration edges, Studio Ghibli restraint, no anime faces
- **Palette:** ink black, rice cream, koi red-orange-white, lantern gold, moon blue, lotus pink
- **Camera:** top-down orbital, shallow depth of field, ripples as primary UI affordance
- **Motion:** slow, ceremonial, never rushed. All UI transitions are water-like.

## Target Audience (DELIBERATELY AMBIGUOUS)

The team has three candidate positionings and has not chosen:

- **A** — Cozy game audience (Stardew, Animal Crossing, Cozy Grove)
- **B** — Mindfulness / reflection app audience (Headspace, Finch, Kind Words)
- **C** — Collectible-social audience (Neko Atsume, Pokémon GO postcards, Sky: Children of the Light)

The founders believe the right answer is "all three, sequenced." They would like the advisory panel's opinion on whether that is courageous or a positioning failure.

## Launch Markets (first 18 months)

Deliberately heterogeneous to stress-test the design:

- **Germany** — GDPR hard mode, privacy-literate audience
- **Japan** — Cultural home, highest stakes for authenticity
- **United Kingdom** — Post-GDPR, Online Safety Act age-gating
- **Brazil** — LGPD, Portuguese-language haiku challenges, different monetization tolerance

**Excluded at launch:** United States (COPPA + state-level complexity), South Korea (real-name ID + loot-box law nuances), China (publishing license), India (data localization).

## Age Rating Deep Dive

Target: **12+ / PEGI 12 / IARC equivalent.**

Under-13 play requires:
- Parental gate
- No city-level location
- No outbound messages
- Their koi travel only to a closed "calm waters" pool of other under-13 players
- Pre-written haiku from a curated bank only

## Hard Constraints (v1 brief, non-negotiable)

1. No text chat, ever
2. No free-form text outside the haiku form
3. No ads
4. No gacha, no loot boxes, no pay-to-speed
5. No profiles, no usernames, no follower graph
6. Cultural consultancy sign-off on all Japanese-origin assets
7. City-level location only, or opt-out to "afar"
8. On-device moderation pass before any message leaves the phone
