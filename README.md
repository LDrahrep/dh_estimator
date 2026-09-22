# Racks, Links, Meters

Demo of a rough labor estimator for rack installation, cable pathways and
structured cabling, in the ISTOK Group visual style. Built for a management
review; it is not used for real estimates and the rates in it are examples.

A single static page: `index.html` holds the markup, styles and script.
No build step, no server, no dependencies. Inputs and edited rates are kept in
the browser (`localStorage`) and can be shared as a link, which encodes them in
the URL after `#s=`.

## Run locally

```sh
python3 -m http.server 4173 --bind 127.0.0.1
```

Then open http://127.0.0.1:4173.

## Deploy

Static project on Vercel, team IstokDevTeam:

```sh
vercel deploy --prod
```

Search engines are kept out on purpose: `robots.txt`, a `noindex` meta tag and
an `X-Robots-Tag` header from `vercel.json`.
