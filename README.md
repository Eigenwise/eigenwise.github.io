# eigenwise.github.io

Account site for the Eigenwise GitHub organization. It holds static redirects and nothing else.

## Why this exists

The Tesseron repository moved from `Eigenwise/tesseron` to `tesseron-dev/tesseron`, and its docs moved with it. Old links to `https://eigenwise.github.io/tesseron/...` would 404 otherwise, so this site forwards them.

## Where the docs are now

https://tesseron-dev.github.io/tesseron/

## What it does

- `/tesseron/` goes to the new docs landing page.
- Any other `/tesseron/...` path (handled by `404.html`) goes to the same path on `tesseron-dev.github.io`, with the query string and hash kept exactly as they were.
- `/` goes to https://eigenwise.io.
- Every other unknown path shows a 404 page with a link to https://eigenwise.io.

Redirect targets are hard-coded to `eigenwise.io` and `tesseron-dev.github.io`. Nothing in the URL can choose a different host. No trackers, no dependencies.

## Ownership

This is an official Eigenwise site, owned and run by Eigenwise (https://eigenwise.io, kenny@eigenwise.io).
