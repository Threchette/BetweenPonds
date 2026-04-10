# 02 — Winter Hibernation

**Image file:** `02-winter-hibernation.png`
**In-game moment:** The pond's state during real-world winter season in the player's hemisphere
**Screen context:** Persistent environmental state for approximately 3 months per year; not an event, a condition

## What Is In The Image

Overhead view of a small koi pond in deep winter at midnight. The pond is surrounded by snow-covered stones. Thin pale ice covers most of the water's surface, textured with subtle cracks and variations — it is real ice, not a stylized placeholder. In the center of the pond is a small clear opening where the ice has not formed, roughly the size of a saucer.

Below the ice, in the dark open water, several koi are visible. They are not swimming. They hang suspended, motionless, at different depths. Their patterns are muted by the darkness of the water and the ice filtering the view. They are alive, but they are sleeping.

On the snowy stone edge of the pond sits a small red paper lantern, lit from within. It glows softly and casts warm amber light across the snow immediately around it. The lantern is the only source of warm color in the entire frame. Beside the lantern, on the snow, sits a small origami crane folded from rice paper.

Snow is falling in the scene — soft, slow flakes visible against the dark background. The overall palette is deep midnight blue for the water and sky, pale blue-white for the ice and snow, and one saturated spot of warm red for the lantern. A single pine branch intrudes from the upper-right corner, its needles dusted with snow.

## Game Design Purpose

Between Ponds follows real-world seasons in the player's hemisphere (determined at first launch via approximate location). Winter is not an event, not a limited-time promotion, not a holiday theme. It is a real condition the pond enters for approximately three months each year and does not leave until the real calendar season changes.

Several deliberate design decisions are embedded in this frame:

- **Koi hibernation is a visible game state.** Players cannot "speed up" winter. They cannot pay to thaw the pond. They cannot force breeding during hibernation. The fish are sleeping, and they will sleep until spring.
- **The activity envelope shrinks.** During winter, koi do not accept new messages to carry (travel slows), breeding is suspended (koi do not breed in cold water), and visitors from other ponds arrive less frequently. The game is deliberately quieter for three real months of the year.
- **The game is still playable.** Players can still feed the koi (less food needed), still tend the pond, still rearrange landscaping, still visit the Memory Wall, still receive and read messages that arrive, and still compose new haiku to release when spring comes. The game does not become zero-activity — it becomes low-activity.
- **The lantern is the player's presence.** That single red glow is the visual signal that someone is still tending this pond even in its quietest season. If a player abandons the pond during winter, the lantern goes out. If the lantern is out for 30 days, the Drift Away mechanic triggers even in winter.
- **The origami crane is a player-made object.** Origami elements appear throughout Between Ponds as small craft objects players can fold (via a minigame) from leftover scroll paper. The crane in this frame was placed there by the player as part of winter landscaping. Other foldable objects include boats, frogs, and lanterns of increasing complexity.

## Seasons Mechanic Details

- **Northern hemisphere players** enter this state roughly December–February.
- **Southern hemisphere players** enter it roughly June–August.
- **Equatorial players** (no clear winter) receive a modified "dry season" equivalent that slows activity less dramatically.
- **Season detection** uses device timezone + the city-level location granted at first launch. Players who opt out of location default to Northern hemisphere seasons and can manually override in settings.

## Key Emotional Register

The designers intend this state to feel like *the quiet room in a house full of activity*. Not empty, not dead, not broken — just resting. Playtesters have described winter mode as "the best reason to come back in spring" and "the part where I missed my pond the most."

## What A Reviewer Might Ask About This Frame

- Is three months of reduced activity a retention risk or a retention feature?
- Does the hemispheric inversion create an unequal experience for Southern hemisphere players during Northern launch windows?
- Is winter playable enough for players who primarily engage during those months due to regional school / work calendars?
- What happens to the Drift Away mechanic during winter — does the 30-day inactivity trigger still apply, and is that fair?
- Does the "lantern is player presence" metaphor hold up, or is it a post-hoc rationalization?
