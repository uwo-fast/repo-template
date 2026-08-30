# Licensing

<!-- Replace YEAR and the project name below.
     Pure-software repository? Delete this file and LICENSES/, keep the root
     LICENSE, and follow the note in the README's License section. -->

Copyright © YEAR Project Name and its contributors

This document summarises how this repository is licensed. It is a summary for
convenience and is **not** a licence itself — the binding terms are the full texts
in [`LICENSES/`](LICENSES/).

This project contains both software and hardware design files, which are licensed
under different open-source licences:

- **Software** — GNU General Public License v3.0 or later (`GPL-3.0-or-later`) —
  [`LICENSES/GPL-3.0-or-later.txt`](LICENSES/GPL-3.0-or-later.txt)
- **Hardware** — CERN Open Hardware Licence Version 2, Strongly Reciprocal
  (`CERN-OHL-S-2.0`) — [`LICENSES/CERN-OHL-S-2.0.txt`](LICENSES/CERN-OHL-S-2.0.txt)

The root [`LICENSE`](LICENSE) is a copy of the GPL text. GitHub reports only one
licence per repository and reads that file, so this document is where the full
picture lives.

## What applies where

Adjust the table to the directories this repository actually uses.

| Path | Licence |
| --- | --- |
| `software/`, `firmware/`, scripts and build tooling | `GPL-3.0-or-later` |
| `cad/` — parametric CAD **source** (`.scad`, CadQuery, build123d) | `GPL-3.0-or-later` |
| `hardware/` — schematics, PCB layouts, gerbers, fabrication outputs | `CERN-OHL-S-2.0` |
| `cad/` — generated geometry (STL, STEP, 3MF), drawings, bill of materials | `CERN-OHL-S-2.0` |
| `docs/` | follows the component documented; general docs are dual, at your option |

Parametric CAD source is treated as software because it is compiled and routinely
includes GPL-licensed libraries, which `CERN-OHL-S-2.0` cannot be combined with.
Where a generated output incorporates geometry from a third-party GPL library, that
output is `GPL-3.0-or-later` as well. See the organization
[licensing policy](https://github.com/uwo-fast/.github/blob/main/LICENSING.md).

## Third-party components

Anything vendored or included keeps its own licence, unaffected by this document.
List it here and keep the list current.

| Component | Licence |
| --- | --- |
| _e.g._ NopSCADlib | `GPL-3.0` |

## Contributions

"Contribution" means any work of authorship intentionally submitted for inclusion
in this project — a pull request, patch, commit, issue, or other communication —
excluding anything conspicuously marked "Not a Contribution".

Unless you state otherwise, contributions you submit are licensed under whichever
of the licences above covers the files they touch, with no additional terms. By
submitting a contribution you represent that you have the right to license it on
those terms.

## Patents

Both GPL-3.0 (section 11) and CERN-OHL-S-2.0 (section 7) contain express patent
provisions. Review them before using, modifying, or distributing this project.

## Disclaimer of warranty and liability

A summary — the full terms are GPL-3.0 sections 15–16 and CERN-OHL-S-2.0 section 6.

THIS PROJECT, INCLUDING ALL SOFTWARE AND HARDWARE DESIGNS, IS PROVIDED "AS IS"
WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, AND
NON-INFRINGEMENT.

HARDWARE DESIGNS HAVE NOT BEEN INDEPENDENTLY VERIFIED OR CERTIFIED FOR SAFETY OR
REGULATORY COMPLIANCE. ANY PHYSICAL PRODUCT MANUFACTURED FROM THESE DESIGNS IS
PRODUCED ENTIRELY AT YOUR OWN RISK. THE AUTHORS AND CONTRIBUTORS ARE NOT
RESPONSIBLE FOR ANY PERSONAL INJURY, PROPERTY DAMAGE, OR OTHER HARM RESULTING FROM
THE USE OR MANUFACTURE OF PRODUCTS BASED ON THEM.

IN NO EVENT SHALL THE AUTHORS, CONTRIBUTORS, OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES, OR OTHER LIABILITY ARISING FROM, OUT OF, OR IN CONNECTION WITH THIS
PROJECT.

## Trademarks

Neither licence grants trademark rights. This project does not grant permission to
use the names, trademarks, or logos of the FAST research group, Western University,
or the project's contributors, except as needed to describe the project's origin.

## Precedence

Where this summary and the full licence texts conflict, the full texts prevail.
