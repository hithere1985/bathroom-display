# Bathroom Display

Morning weather page for a Seeed reTerminal E1001 e-paper display mounted in the bathroom.

## How it works

- `index.html` is a single self-contained 800x480 page, published with GitHub Pages.
- SenseCraft HMI renders the page through its Web Content feature, using the GitHub Pages URL.
- Weather data comes from the [Open-Meteo](https://open-meteo.com/) forecast API (no API key required).

## Changing the location

Edit the `LAT`, `LON`, and `TZ` constants at the top of the script in `index.html`:

```js
const LAT = 43.3178, LON = -88.3790, TZ = "America/Chicago";   // Hartford, WI
```

`TZ` must be an IANA time zone name. Commit and push to `main`; GitHub Pages redeploys automatically.

## Commit messages

Short imperative style, e.g. `Update location to Milwaukee`.
