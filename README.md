## Ray Ma

Software developer at Prairie Robotics, in Saskatchewan. I build small, fast web tools, and I gravitate toward problems where the hard part is getting the numbers right.

### Compass

Seven calculator sites for home and vehicle costs. Shared engine, separate domains, each one built around a question people actually type into a search bar. Astro, deployed on Cloudflare Pages.

| Site | What it answers |
| --- | --- |
| [YardCompass](https://yard-compass.com) | How much mulch, gravel, topsoil, or sod a yard actually needs |
| [RoofCompass](https://roof-compass.com) | Roof replacement cost, measurement, and what insurance will cover |
| [SepticCompass](https://septic-compass.com) | Septic tank sizing, drain field, and total system cost |
| [FoundationCompass](https://foundation-compass.com) | Foundation and basement repair cost, and whether it is a covered claim |
| [MoldCompass](https://mold-compass.com) | Mold and water damage remediation cost |
| [SewerCompass](https://sewer-compass.com) | Sewer and water service line cost and claims |
| [DriveCompass](https://drive-compass.com) | Gas, loans, leases, and what an EV really costs to run |

Regional pricing is derived from BLS wage data rather than guessed, which is most of the work.

### Tools

**[gsc-weekly-brief](https://github.com/RayWangyangMa/gsc-weekly-brief)** — the Monday-morning automation behind the sites above. Pulls every Search Console property through the API, keeps the history Search Console itself throws away, diffs the last two pulls, and writes one short brief that flags only the pages actually worth acting on. Live-checks each candidate first, because "great position, lots of impressions" is bad advice when the URL is a 404.

### Open source

Merged into **[openclaw/openclaw](https://github.com/openclaw/openclaw)**:

**[#135516](https://github.com/openclaw/openclaw/pull/135516)** — cron failure alerts fired and forgot. The send's outcome was never written back, so `cron get` answered `unknown` forever and a broken alerting path was invisible — the one place you least want silence. The settled result is now committed back to the live job (delivered, or not-delivered with a redacted reason), guarded against sibling services on the same store and against writes SQLite refused. Proven both ways against a real gateway.

**[#134780](https://github.com/openclaw/openclaw/pull/134780)** — the plugin registry kept reporting `source-changed` drift against plugins that had not changed. Two equivalent record shapes normalized differently, so a strict comparison never matched. Fixed the normalizer and reproduced the whole thing end to end against a real CLI; the maintainer took the same fix further into the inventory fingerprint cache.

### Elsewhere

Off the clock I run a self-hosted home stack — a control dashboard, 3D printer automation, and a small pile of devices that talk to each other more than they strictly need to.

[rayma.ca](https://rayma.ca) · [LinkedIn](https://www.linkedin.com/in/ray-wangyang-ma/)
