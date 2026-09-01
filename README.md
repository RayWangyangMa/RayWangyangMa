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

### Open source

**[openclaw/openclaw](https://github.com/openclaw/openclaw)** — [#134780](https://github.com/openclaw/openclaw/pull/134780)

The plugin registry kept reporting `source-changed` drift against plugins that had not changed. Two equivalent record shapes normalized differently, so a strict comparison never matched. Fixed the normalizer and reproduced the whole thing end to end against a real CLI; the maintainer took the same fix further into the inventory fingerprint cache.

### Elsewhere

Off the clock I run a self-hosted home stack — a control dashboard, 3D printer automation, and a small pile of devices that talk to each other more than they strictly need to.

[rayma.ca](https://rayma.ca)
