# Tech Performance Hub

A five-page static website that explains gaming PC troubleshooting, compares example hardware configurations, and demonstrates performance calculators using HTML, CSS, and vanilla JavaScript.

Built by **Hanoch Sabu**. This project demonstrates technical documentation, user-facing support guidance, and basic front-end development. It is an educational prototype; it does not measure or optimize a user's computer.



## Run locally

Requirements: a modern browser. Python 3 is optional for serving the site locally. No packages, API keys, database, or build step are required.

```sh
git clone https://github.com/HanochSabu/Gaming-Optimization-Website.git
cd Gaming-Optimization-Website
python3 -m http.server 8000 --bind 127.0.0.1
```

Open <http://localhost:8000>. Stop the server with Ctrl+C. If port 8000 is busy, use 8001 and update the URL. You can also open `index.html` directly in your browser. Home-page photos load from Unsplash and require internet access; the guides and calculators run locally.

## Features and source map

| Page | What it implements |
| --- | --- |
| `index.html` | Landing page, featured guide cards, example build comparison, and navigation |
| `performance.html` | Windows, GPU, network, and in-game guidance; comparison table and pre-game checklist |
| `builds.html` | Three example build tiers and a CPU/GPU/RAM/game selector with a JavaScript calculation |
| `optimization.html` | Illustrative before/after table and system/optimization-level calculator |
| `contact.html` | Link to GitHub Issues for public project feedback; no message collection |

Styles and scripts are inline in their respective HTML files. There are no framework or server dependencies.

## Calculator behavior and limits

**Build calculator (`buildPC`):** starts at 70, 120, or 200 FPS for the three GPU choices; adds 15 or 30 for selected CPUs, adds 10 for 32GB RAM, then applies a game adjustment (-50 to +40). The resulting number selects a settings label at thresholds of 80 and 140 FPS. These are hard-coded rules, not benchmark data, hardware detection, or compatibility validation.

**Optimization calculator (`optimizeCalc`):** starts at 20, 30, or 15 FPS for low-, mid-, or high-end systems, and adds 20 for advanced optimization. These values illustrate conditional logic and are not evidence of actual performance gains.

The tables also contain illustrative values. No test rig, resolution, driver version, repeatable benchmark, or measured before/after results are supplied. Network latency in milliseconds is distinct from FPS. Do not use this prototype alone for purchasing decisions.

## Screenshots

Screenshots are still needed: capture the home page and a populated build calculator at desktop and mobile widths. Browser capture was blocked by the review environment; no simulated screenshot is presented as application evidence.

## Verify the project

1. Open all five pages through the navigation; confirm each link reaches the expected page.
2. On PC Builds, select Ryzen 5 5600 / RTX 2060 / 16GB / Fortnite. Click **Estimate Performance**: the example should return **90 FPS**, Medium–High Settings.
3. Select Ryzen 7 7800X3D / RTX 5090 / 32GB / Cyberpunk 2077: expect **190 FPS**, High / Ultra Settings.
4. On Optimization, select Low-End PC / Basic Optimization: expect **+20 FPS**. High-End PC / Advanced Optimization should return **+35 FPS**.
5. At a narrow browser width, confirm navigation wraps and tables scroll within their containers. Tab through links, selectors, and buttons; results announce through live regions.
6. On Contact, confirm the GitHub Issues link appears and no form suggests a message was delivered.

See [the portfolio review](docs/portfolio-review.md) for priorities, validation scope, and resume wording.

## Portfolio relevance

- **IT and technical support:** explains Windows, GPU, and network troubleshooting concepts in user-facing guides and checklists.
- **Development:** implements a five-page site and two interactive JavaScript calculators without a framework.
- **Cybersecurity:** this repository does not implement security monitoring, vulnerability scanning, authentication, or incident response. Present it as a support/documentation project rather than a cybersecurity tool.

## Next improvements

Replace illustrative values with reproducible measurements and source citations; add structured troubleshooting cases with symptoms, diagnostic steps, rollback, and verification; consolidate shared styles; and add automated navigation/calculator checks. A deployed demo would help reviewers, but no deployment is asserted here.
