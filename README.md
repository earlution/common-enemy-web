# common-enemy-web

Public landing site for **A Common Enemy** — podcast and analysis by Ruari Mears.

**Live (after first deploy):** https://earlution.github.io/common-enemy-web/

**Production canon** lives in the private repo [earlution/common-enemy](https://github.com/earlution/common-enemy). This repo publishes only marketing-facing static pages.

---

## Branches

| Branch | Role |
| ------ | ---- |
| **dev** | Day-to-day edits; push as often as you like — **no** GitHub Pages deploy |
| **main** | Production; merge from dev after local preview; push **triggers** Pages deploy |

```bash
git checkout dev
python3 -m http.server 8080
# open http://localhost:8080
git checkout main && git merge dev && git push origin main
```

---

## Enable Pages (once)

**Settings → Pages → Source:** GitHub Actions

---

## Phase 1 checklist

- [x] Site scaffold (hub, methodology, about)
- [ ] Newsletter provider embedded on `index.html`
- [ ] SocArXiv URL wired when preprint is live
- [ ] YouTube segment URLs in `methodology.html` after recording
- [ ] Podcast feed link when host is configured

See `marketing-strategy-v0.1.2.md` in common-enemy (Phase One / Campaign A).

---

## Related

| Repo | Role |
| ---- | ---- |
| [earlution/common-enemy](https://github.com/earlution/common-enemy) | Private — scripts, docs, production |
| [RMS-Ltd/web](https://github.com/RMS-Ltd/web) | Cooperative umbrella — optional cross-link only |
