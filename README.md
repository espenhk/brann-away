# brann-away

Brann away trips, live at <https://espenhk.github.io/brann-away/>.

Published by the `brann-away-trip` Claude skill, which commits straight to
`main`. Everything here is encrypted (AES-256-GCM, key from PBKDF2-SHA256 of a
master password); nothing readable about a trip is ever committed.

- `kdf.json` — site salt and PBKDF2 parameters (not secret)
- `manifest.enc.json` — encrypted list of trips
- `index.html` — encrypted index page
- `<slug>/index.html` — one encrypted page per match

Don't edit these by hand; rerun the skill for the match instead.
