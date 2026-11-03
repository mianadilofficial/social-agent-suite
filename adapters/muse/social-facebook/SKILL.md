# Social Facebook (Muse adapter)

Run the Facebook module (`platforms/facebook/SKILL.md`) through Muse's
hands: the signed-in browser on the owner's PROFILE (never the Page).

## When to use

The owner asks for a Facebook post, comment replies on his profile, or
light engagement.

## Route notes

- The browser cannot attach images to profile posts: prepare the text,
  hand the image step to the owner, publish the rest. Report the pattern
  plainly instead of working around it silently.
- Comment handling follows the owner's reply rule in the module
  (reply / like-only / surface-to-owner).
- No connector route exists for profiles — browser only, human pace,
  stop on any checkpoint or warning.

The module holds the full rules. Follow it.
