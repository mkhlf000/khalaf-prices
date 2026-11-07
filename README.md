# Khalaf material prices

`prices.json` feeds the Material prices page of the Khalaf portal (https://khalaf-portal.web.app).
It is refreshed daily by a scheduled Claude task from published Egyptian market reports.

Format: `{updated, note, items:[{id, g, en, ar, u, uAr, key, h:[{d, p, lo?, hi?, src, url?}]}]}`
- `g` group: steel | cement | concrete | brick | agg
- `h` history, oldest first; one entry per date; prices in EGP.
