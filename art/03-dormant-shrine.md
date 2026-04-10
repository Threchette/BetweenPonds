# 03 — Dormant Shrine

**Image file:** `03-dormant-shrine.png`
**In-game moment:** The Memorial Pond state — the pond of a player who has been inactive for 180+ days
**Screen context:** Visible to *other* players when their koi visit this pond; the dormant player does not see this view unless they return

## What Is In The Image

A small koi pond seen from a low three-quarter angle — much closer to eye level than the other pond frames. Cool overcast autumn light; the sky implied beyond the frame is grey, not golden. There is no moon visible and no time-of-day dramatic lighting. The effect is ordinary afternoon light on an ordinary day.

Moss has grown heavily over the stones surrounding the pond. Some of the moss is clearly established — this is not a newly neglected pond, this is one that has been in this state long enough for moss to take hold. Lotus leaves crowd much of the water's surface on the left side of the frame, larger and more spread than the curated arrangements seen in active ponds.

Fallen maple leaves in deep red and orange float on the dark, still water. A few more leaves are suspended in the air, still falling. The water is dark and reflective but absolutely still — there is no visible ripple, no movement, no wake.

To the left of the frame, a stone lantern stands, leaning very slightly. A faint spiderweb is draped across one of the lantern's open windows. The web is not elaborate and not ominous — it is the kind of web a small spider builds in a week and abandons.

On the right side of the frame, a weathered wooden post stands at the edge of the pond. A single rice-paper scroll is pinned to the post with a small nail. The scroll is torn along one edge, yellowed with age, curling at the top and bottom. It has not been replaced in a long time.

Swimming alone through the scene, circling slowly, is a single bright-gold koi. The koi is clearly a visitor — it is not patterned, not paired with others, and its bright color contrasts sharply with the muted palette of the rest of the frame. It appears to be moving slowly and somewhat hesitantly, not certain whether to stay.

The palette is dominated by moss green, wet stone grey, deep water black, and the muted reds and yellows of autumn leaves. The gold koi is the only bright accent.

## Game Design Purpose

This frame depicts the **Memorial Pond** state, which is one of the three "darker mechanics" in the game's brief. When a player has been inactive for 180 consecutive days, their pond transitions into this state:

- The player's own koi become visible but no longer release. The player, if they return, must first "wake" the pond before they can send again.
- Visiting koi from other players can still arrive. This is crucial — the dormant pond is not walled off from the rest of the game's network.
- When a visiting koi arrives, *its* player (the sender) sees the dormant pond state in the arrival animation. This frame is roughly what that sender sees when their koi has been delivered to a dormant pond.
- The dormant pond's owner can return at any time and "wake" the shrine, at which point the pond transitions back to its active state over the course of a few days. Mosses recede, leaves clear, new scrolls can be pinned.
- If the player permanently quits and requests account deletion (GDPR erasure), the Memorial Pond is removed from the visitable network entirely and any koi that were mid-journey to it are redirected to the "afar" pool.

## The Ambiguity Is Deliberate

The art direction for this frame was explicitly revised from an earlier warmer version because the original felt too clearly peaceful. The design intent is that a viewer — whether a player, a reviewer, or a critic — should not be able to confidently decide whether this pond is being *patiently tended from elsewhere* or *quietly forgotten*.

The specific visual signals of ambiguity:

- **The spiderweb** could mean "nobody tends this" or could mean "the caretaker chose not to sweep it because small creatures have a right to build homes too."
- **The torn scroll** could mean "nobody has replaced this in months" or could mean "the last message the caretaker pinned is still here because they wanted it to stay."
- **The moss** could mean "this place is unkempt" or could mean "this place has been allowed to grow wild on purpose."
- **The solo visiting koi** could mean "this pond is lonely" or could mean "this pond still receives visitors, which is the whole point of the game."
- **The overcast light** could mean "this is a sad place" or could mean "the day is simply not a dramatic one."

Every visual element is deliberately dual-coded.

## Game Design Decisions Visible Here

- **Memorial Ponds are visitable, not hidden.** The game deliberately exposes the dormant state to other players. It does not pretend dormant ponds don't exist. This is part of the game's philosophy about impermanence.
- **Visiting koi can still deliver messages.** A player's haiku can still reach a dormant pond. The dormant player may return in six months and find a stack of messages waiting.
- **Nothing decays.** The pond does not become ugly. The koi do not die. The fish do not escape. The game refuses to punish the player for leaving.
- **The "Last Koi" rule still applies.** Even in a Memorial Pond, the final koi can never be sent away. If a player returns after two years, their oldest original koi is still there.

## Key Emotional Register

The designers intend this state to feel *neither peaceful nor tragic*. They want it to feel *patient*. Playtesters have split sharply on this frame — some have described it as the most beautiful screen in the game, others have described it as "deeply sad in a way I can't explain." The designers consider both reactions to be the correct reaction.

## What A Reviewer Might Ask About This Frame

- Is the Memorial Pond a humane piece of sunset UX, or is it a psychological trap for players who already quit?
- Is showing the dormant state to other players a form of shaming, or a form of respect?
- Does the "wake the shrine" return mechanic create a FOMO hook that compromises the stated philosophy of impermanence?
- Is the visual ambiguity defensible, or is it a rationalization for a dark retention pattern dressed up as art direction?
- What are the legal implications of preserving a dormant player's in-game state visible to others under GDPR, particularly for minors who age out of the 12+ audience?
- Does the Memorial Pond create unequal experiences for visiting players — some ponds dormant, others active — in a way that affects core gameplay for everyone?
