# Buzz In

A no-backend, peer-to-peer buzzer game. One phone hosts, any number of
phones join as contestants, first tap wins the round. Runs entirely as
static files — no server, no account, no database to maintain.

It uses [PeerJS](https://peerjs.com/) so devices connect directly to
each other; PeerJS's free public service is only used for the initial
handshake. Works best when everyone is on the same WiFi.

## Deploy to GitHub Pages (one-time setup, ~2 minutes)

1. Go to [github.com/new](https://github.com/new) and create a new
   repository (public or private both work), e.g. `buzz-in`.
2. On the new repo's page, click **"uploading an existing file"** and
   drag in `index.html` from this folder. Commit it.
3. Go to the repo's **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a
   branch`, branch `main`, folder `/ (root)`. Save.
5. GitHub shows your live URL at the top of that page after a minute
   or two, usually `https://<your-username>.github.io/buzz-in/`.

That URL is what you open to host, and what you share with
contestants to join — same link for both, they just pick "Host a
game" or "Join a game" on the landing screen.

## Using your own domain instead

If you'd rather it live at your own domain: in the same **Settings →
Pages** screen there's a "Custom domain" field — enter it there, then
add a `CNAME` record at your DNS provider pointing that subdomain to
`<your-username>.github.io`. GitHub will show you the exact record to
add.

## Updating it later

Edit `index.html` in the repo (or re-upload a new version) and commit
— GitHub Pages redeploys automatically within a minute or so.
