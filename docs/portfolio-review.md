# Portfolio readiness review

## Highest-value improvements

| Priority | Finding | Action in this pass |
| --- | --- | --- |
| 1 | No README or setup instructions | Added overview, file map, local server instructions, dependencies, limits, and verification steps |
| 1 | Hard-coded FPS values read like measured outcomes | Labeled example tables and calculator output as illustrative; documented exact rules |
| 1 | Contact form had no handler or backend | Replaced it with a working GitHub Issues link and clear static-site explanation |
| 2 | No screenshots | Pending: browser launch was blocked by the review environment; capture home and populated calculator views |
| 2 | Missing viewport metadata and narrow-screen handling | Added language/charset/viewport metadata, wrapping navigation, scrollable table containers, and mobile spacing |
| 2 | Select labels were unassociated and results had no live announcement | Associated labels, added live regions and visible keyboard focus |
| 3 | Repeated inline CSS and no automated checks | Documented as follow-up; retained the original architecture |

## Suggested GitHub About description

Five-page HTML/CSS/JavaScript gaming PC support prototype with Windows/GPU/network guides, example build comparisons, and two illustrative performance calculators.

Suggested topics: `html`, `css`, `javascript`, `technical-support`, `pc-hardware`, `portfolio`.

The repository description/topics are settings outside the source tree; the text above is ready to copy into GitHub About.

## Resume-ready bullets

Use only if you can explain and take ownership of the implementation:

- Developed a five-page HTML, CSS, and JavaScript website presenting Windows, GPU, and network performance guidance through comparison tables and troubleshooting checklists.
- Implemented two browser-based demonstration calculators using hardware/game selections and conditional logic; documented calculation rules and limitations to distinguish simulated outputs from measured benchmarks.
- Improved project usability and handoff with local setup instructions, mobile navigation, scrollable tables, associated form labels, and keyboard focus indicators.

Do not claim measured FPS gains, customer adoption, production deployment, compatibility validation, or security tooling: the repository provides no evidence for those outcomes.

## Best next project extension

Add one reproducible support case: record the symptom, system configuration, baseline FPS or network latency, diagnostic steps, one controlled change, rollback procedure, and repeated results under the same conditions. Keep real measurements separate from the demonstration calculators. This would provide stronger interview evidence for technical support work.

## Validation and remaining checks

The calculator scripts were executed with a minimal DOM fixture in Node.js for all selectable combinations, and local navigation targets and metadata were checked. These checks do not validate browser layout, accessibility behavior, or screen-reader output. Browser launch was blocked by the environment (socket operation not permitted), so visual QA and screenshots remain outstanding. The README includes manual browser verification steps.
