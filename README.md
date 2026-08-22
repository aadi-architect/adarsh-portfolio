# Aadi Adarsh — Portfolio

Personal site for **Aadi Adarsh** (Adarsh Kumar), applied AI engineer working on
identity-continuity systems, long-term memory architecture, and affective computing
(CCCS · Project SIM).

Live: **[aadiadarsh.dev](https://aadiadarsh.dev)**

## Contents

| File | Purpose |
| --- | --- |
| `index.html` | The entire site — markup, styles, and the CCCS layer selector, no build step |
| `og.png` | 1200×630 social preview card |
| `favicon.svg` | Tab icon |

## Local preview

```sh
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploying

Static — deploy the folder as-is. Production is Vercel, served from the apex domain
`aadiadarsh.dev` (with `www` 308-redirecting to apex).

## Notes for editing

- **Canonical origin** is set in two places near the top of `index.html`, marked with a
  comment block. Change both if the domain ever moves.
- **CCCS layer copy** lives in the `layers` array in the inline script — the panel, the
  list, and the progress bars all render from it, so edit it there and nowhere else.
- **Metrics** are split into *Measured* and *Design targets* groups. Keep that separation:
  measured numbers come from the documented N=1 session, targets are thresholds the
  R-Score is designed against.
