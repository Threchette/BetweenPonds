# 06 — Message Board (Memory Wall)

**Image file:** `06-message-board.png`
**In-game moment:** The Memory Wall — the player's accumulated archive of messages received from strangers
**Screen context:** A separate screen the player navigates to from their pond; not the default view

## What Is In The Image

The interior of a traditional wooden pavilion at dusk. The view is from inside the room looking toward the back wall, with the open exterior visible through a sliding door on the right side of the frame.

The back wall is almost entirely covered by a large, stylized flat world map rendered in pale ink on aged parchment-colored paper. The map is not geographically precise — it is an artistic representation, closer to an old maritime chart than a modern political map. The continents are recognizable (North and South America, Europe, Africa, Asia, Australia) but their borders are softened and their interiors are mostly blank. A compass rose with a decorative sun pattern sits in the lower-left quadrant of the map. A few small stylized mountain and wave illustrations decorate otherwise empty areas.

Pinned to the map at various locations are dozens of small rice-paper scrolls. Each scroll is roughly the size of a playing card, rolled or flat. Each scroll is marked with a single red wax seal. Some scrolls are crisp and white; others are yellowed or weathered. The scrolls are pinned at what appear to be their approximate city or country of origin — some in North America, several in Europe, some in Africa, several in Asia, one in Australia, a few in South America.

On the wooden floor in the foreground, two small paper lanterns glow softly, casting warm amber light upward onto the map. The light emphasizes certain scrolls more than others — the lantern positions create a reading path, not a flat wash.

Through the open sliding door on the right, a moonlit garden is visible — the edge of what may be the player's own pond is suggested in the darkness beyond. A faint koi-shaped shadow drifts across the floor's reflection near the door, suggesting the game's world continues just beyond the view.

The palette is dominated by the warm cream of the aged paper, deep wood-brown for the walls and floor, pale ink for the map details, and the small points of amber light from the lanterns. The red wax seals are the only saturated color in the scene.

## Game Design Purpose

This is the **Memory Wall** — the second primary screen of Between Ponds after the pond itself. It is where the player stores every message they have ever received from a stranger.

Visible design decisions:

- **Received messages are preserved; sent messages are not.** When a player releases a koi with a composed haiku, the scroll is gone from their world — they cannot re-read what they wrote. But when a stranger's koi arrives in the player's pond carrying a haiku from somewhere else, that scroll is archived here on the Memory Wall forever (or until the player chooses to "release" it back into the current). This is a deliberate asymmetry. The game wants players to remember what they were given, not what they gave.
- **Pinned at origin.** Each scroll is pinned to the approximate city or country it came from, based on the sender's city-level location (or "afar" if they opted out). Over months and years, a player's Memory Wall develops a visible pattern — a cartography of their accumulated contacts.
- **The seals are unique per player.** Each player's wax seal is a small procedurally-generated pattern based on their initial pond configuration. When a scroll arrives from a new sender, the seal is new. When another arrives from the *same* sender later (a rare event), the seal matches. This is the closest Between Ponds comes to a "friend list" — you can tell if a new message is from someone you have heard from before, but you have no other identifying information about them.
- **No readable text.** The scrolls on the Memory Wall do not display the text of the haiku when viewed at this scale. The player must tap a scroll to open it and read the message individually. This is deliberate — the wall is for *presence*, not for scanning. Reading 40 haiku at once is not the point.
- **The lanterns are player-placeable.** Players can purchase and place lanterns on the floor to illuminate specific regions of the map. A player who has received many messages from Brazil may choose to place a lantern in that region to give it visual emphasis. This is a form of self-curation.
- **The exterior view is the player's own pond.** The door on the right always opens onto whatever state the player's pond is currently in. At night, moonlit. In winter, snowed over. At dawn, misted. This connects the two primary game spaces visually — the pond and the wall are not separate screens but different rooms in the same place.

## What The Memory Wall Is Collecting

This is worth stating explicitly because it is the answer to the question *"what is the progression system of this game?"*

Between Ponds has no leveling system. No experience points. No skill tree. No unlock grid. No daily quests with completion percentages. No battle pass.

The only thing that accumulates over time — the only thing the game tracks as *your record* — is the number of messages you have received from strangers. The Memory Wall is the progression display. Your progress in Between Ponds is measured in evidence that strangers chose to write to you.

## Scroll Interactions

When the player taps a single scroll on the Memory Wall, the scroll enlarges to full screen and the three-line haiku becomes readable. The player can then:

- **Keep** the scroll (default) — it stays pinned on the wall indefinitely.
- **Release** the scroll back into the current — the scroll animates away and becomes a message delivered to a different stranger, with the original sender's haiku intact and a small note that this message has traveled.
- **Fold** the scroll into an origami object (crane, frog, boat, etc.) that the player can then place as landscaping in their pond.

The player cannot delete a scroll. The only options are keep, release, or transform.

## Key Emotional Register

The designers intend the Memory Wall to feel like *a museum that is also a living room.* A space that is both archival and intimate. The mood is meant to invite sitting, not scrolling.

## What A Reviewer Might Ask About This Frame

- Is a collection of messages a sufficient progression system for a free-to-play mobile game, or is this going to feel insubstantial to players who expect visible numeric growth?
- Is the "no delete" rule defensible when a message arrives that contains something the player finds upsetting? What is the escalation path?
- Does pinning scrolls to city-level origins create privacy risk when a player's Memory Wall is screenshotted and shared on social media outside the game?
- Can this screen be meaningfully experienced by a player who is blind or has low vision, given that the primary information is spatial (where on the map the scroll is pinned)?
- Does the asymmetry (received messages preserved, sent messages discarded) create an emotional imbalance where players feel more *taken from* than *given to*?
- What happens to the Memory Wall if the player permanently quits and deletes their account? Are the preserved messages from other players also deleted (GDPR concern) or preserved (respect for the senders)?
