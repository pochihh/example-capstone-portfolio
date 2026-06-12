# Example Capstone Portfolio

This repository is a working example for MAE 162D/E teams. The gallery uses this
page to demonstrate how to fill in `manifest.json` and how to write a README
that becomes a clear project page.

## What The Gallery Uses

The gallery reads three things from each project repository:

| File | Purpose |
| --- | --- |
| `manifest.json` | Short structured metadata for the gallery card and project header. |
| `README.md` | The main project page content. |
| Thumbnail image | The image referenced by `manifest.thumbnail`, cached by the gallery. |

The project page body is rendered from this README. The manifest should stay
short and factual; put the real explanation, figures, design notes, and results
in the README.

## Example Manifest

Place `manifest.json` at the root of your repository:

```json
{
  "schema_version": 1,
  "course": "MAE 162D/E",
  "year": 2026,
  "section": "Tsao",
  "group": 8,
  "title": "Example Capstone Portfolio",
  "authors": ["Example Student", "Example Teammate"],
  "summary": "A sample capstone portfolio that demonstrates how teams should fill in manifest.json and structure their README for the gallery.",
  "thumbnail": "assets/creation_of_robot.png",
  "keywords": ["manifest", "readme", "portfolio"]
}
```

Field notes:

- `schema_version` must be `1`.
- `course` must be exactly `MAE 162D/E`.
- `year` and `group` are numbers.
- `section` should match your instructor section.
- `thumbnail` is a path relative to the repository root.
- `keywords` is optional, but useful for scanning the gallery.

## Recommended README Structure

Use headings so the project page is easy to skim.

## Project Overview

Start with one short paragraph explaining what your team built and why it
matters. A reader should understand the project without opening any other file.

## Problem

Describe the engineering problem, constraints, and target users. Include enough
context for someone outside your team to understand the design choices.

## Design And Approach

Explain the main mechanical, electrical, software, and controls decisions. Use
short subsections if your project has multiple subsystems.

Example:

| Subsystem | What To Explain |
| --- | --- |
| Mechanical | Chassis, actuation, fabrication, mounting, tolerances. |
| Electrical | Sensors, power, wiring, custom boards, safety limits. |
| Software | Architecture, important algorithms, data flow, interfaces. |
| Testing | What you measured, how you validated it, and what changed. |

## Results

Summarize what worked, what did not work, and what you learned. Include numbers
when possible: speed, accuracy, load, runtime, latency, repeatability, or other
performance metrics.

## How To Reproduce

If another team or future student should be able to run your work, include the
minimum steps:

```sh
# Example only. Replace this with commands that apply to your project.
git clone <your-repo-url>
cd <your-repo>
```

Then describe hardware setup, required dependencies, calibration, and launch
commands.

## Team Contributions

List major responsibilities clearly.

| Member | Contributions |
| --- | --- |
| Example Student | Mechanical design, fabrication, validation. |
| Example Teammate | Controls, software integration, documentation. |

## Writing Tips

- Keep the summary in `manifest.json` short.
- Put the real explanation in `README.md`.
- Prefer concrete results over broad claims.
- Use tables for comparisons and responsibilities.
- Use relative paths for repository files.
- Make sure the thumbnail path in `manifest.json` actually exists.
- Keep this README useful even if someone reads it outside the gallery.
