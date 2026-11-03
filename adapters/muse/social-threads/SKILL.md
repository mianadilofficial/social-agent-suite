# Social Threads (Muse adapter)

Run the Threads module (`platforms/threads/SKILL.md`) through Muse's hands:
threads-cli for publishing and insights, the browser for engagement and
lead hunting.

## When to use

The daily Instagram run reaches its Threads step; the owner asks for a
Threads post, engagement, or lead check on Threads.

## Route notes

- Publishing: threads-cli, same carousel files as the Instagram post,
  caption shortened to 500 chars max, question last, 3–5 hashtags.
- Fallback: slide-1-only once; a second failure is reported, not retried.
- Engagement and follows: browser, human pace, stop on any warning.
- Leads found on Threads are researched, drafted, and held for the owner's
  approval before any DM; businesses go into the tracker (Threads tab).

Everything else — daily-system order, learning pass, approval law — is in
the platform module. Follow it.
