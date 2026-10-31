# Taxonomy and working rules

## Names and paths

Use lower-case hyphenated stable IDs: `ford-double-barra-v12`, `ford-au-aeroblade`. File paths are `concepts/<manufacturer>/<id>.md`. Use the original manufacturer as the folder and a separate marque field for badges such as FPV or HSV; this is a filing convention, not a corporate-ownership claim.

Aliases belong in the canonical brief so GitHub search finds names such as “DB12”, “original X-Type” or “GTHO”. Keep prompts inside the brief initially; add a separate prompt file only when there are multiple approved variants. Editorial entries reference the concept ID.

## Metadata

Each concept begins with YAML front matter:

| Field | Meaning / allowed values |
| --- | --- |
| `id`, `title`, `manufacturer`, `marque`, `aliases` | Stable identity and searchable names |
| `kind` | `speculative-reconstruction` or `documented-history` |
| `work_status` | `active`, `parked`, `complete` |
| `research_status` | `needs-sources`, `in-progress`, `checked` |
| `render_status` | `brief-only`, `references-needed`, `in-progress`, `approved`, `not-applicable` |
| `editorial_status` | `idea`, `draft`, `ready`, `published` |
| `updated` | ISO date of the repository brief update |

These statuses are independent. A finished render does not make its historical claims checked or its article ready. `checked` requires evidence for every factual claim intended for release; `approved` requires an inspected asset and recorded approval. Initial statuses describe what this repository can substantiate, not a claim that earlier work never happened.

## Evidence labels inside any file

| Label | Use |
| --- | --- |
| **DOCUMENTED** | Real-world claim supported by a linked source, locator and stated scope |
| **UNVERIFIED** | Research lead, recollection or allegation needing evidence |
| **SPECULATIVE** | Alternate history, invented model, proposed specification or engineering hypothesis |
| **DECISION** | User's creative constraint; records intent, not historical truth |

A speculative vehicle can use documented donor facts: label those claims separately. Recalled chat content establishes creative provenance only; it does not establish automotive history. See the [research standard](research/README.md).

## Small by design

- One canonical brief per concept; family briefs may contain separate generation entries.
- Keep the initial four briefs; promote a parked idea only when it becomes the chosen work item.
- Keep one next step per brief. Avoid creating issues, empty marque folders or a task for every possible variant.
- The documentary order and PUC social order are separate. “Ready” requires completed assets/copy and resolved release blockers; it does not mean scheduled.
- Record original asset links, version/approval and usage permission when available. Never substitute an invented local path or overwrite an approved master.
