# skrrr — US drywall, framing & painting takeoff data brief

## Purpose

This brief defines the evidence needed for AI quantity-takeoff benchmarking in US construction:

**Clean drawings + matching specifications → marked geometry + completed quantities.**

The primary scope is US commercial interiors: offices, schools, healthcare, retail, hospitality, multifamily common areas, and tenant improvements. The unit of analysis is a **project × trade × phase × revision package**.

## Evidence requirements

| Role | Required for an ideal package | Details |
|---|---|---|
| Input | Original, unmarked drawings | Architectural plans, reflected ceiling plans, elevations, sections, details, relevant schedules and sheet index; readable dimensions and scale. |
| Input | Matching specifications | Project-specific trade sections and applicable general requirements; embedded drawing notes count only when their scope is documented. |
| Answer evidence | Marked-up drawings | Measured lines, polygons, counts, legends and labels tied to the same sheets and revision. Prefer editable geometry or annotation exports alongside the visual PDF. |
| Answer evidence | Completed takeoff | XLSX/CSV preferred; quantity report PDF acceptable. Actual quantities, descriptions and units, with scope breakdown and links to geometry where available. A blank template or price-only bid is insufficient. |
| Supporting | Helpful, not universally required | Wall/finish/door schedules, addenda, RFI answers, assumptions/exclusions, measurement rules, scale calibration, annotation layers, software/version, reviewer and provenance. |
| Secondary | Optional commercial information | Labor, productivity, unit prices, waste, equipment and totals. Preserve separately from measured quantities; price evidence cannot replace quantity evidence. |

### Priority trades and quantity distinctions

1. **Drywall and associated framing:** partition types and lengths; wall heights; sides and board layers; board type/thickness; studs, spacing/gauge, tracks and headers; shaft walls; ceilings, soffits and bulkheads; openings and returns; insulation and finish levels when in scope. Retain assembly definitions and distinguish wall length, one-face area, total board-layer area, sheet count and purchase quantity.
2. **Painting:** wall and ceiling surfaces, doors, frames, trim/base, exposed substrates and specialty finishes. Capture substrate, finish system, primer/topcoat counts, room/finish codes, new versus existing surfaces, preparation and exclusions. Distinguish net paintable area from coat-weighted area and gallons derived from coverage/waste.
3. Related interior scopes are useful when they explain these trades. Do not let structural concrete, civil/sitework or generic whole-building cost estimates dominate collection. Residential examples are secondary and must be labeled.

Record units explicitly (SF, LF, EA, sheets, gallons, etc.), original precision and any conversions. Never equate similarly named quantities without checking sides, layers, coats, opening deductions, waste and scope.

## Package tiers and selection

Package completeness and answer correctness are separate axes. A complete vendor example is not automatically gold.

| Tier | Evidence available | Disposition |
|---|---|---|
| A — complete paired | Verified original drawings, matching specifications, marked drawings and completed quantities; same project/trade/phase/revision supported by evidence | Highest collection priority; eligible for expert review, not automatically a trusted benchmark. |
| B — partial paired | Original drawings and completed quantities have credible pairing; specifications or marked drawings are missing/partial | Retain with explicit gaps; benchmark only the supported scope after review. |
| C — answer-side lead | Marked drawings and/or quantities; originals absent or pairing/revision unresolved | Discovery queue; do not claim a clean-input benchmark. |
| D — input-side lead | US drawings/specifications with no completed answers | Useful input inventory; independent takeoff creation would be a separate task. |
| Excluded | Unrelated trades, blank templates, cost-only summaries, unreadable artifacts, non-US projects, fabricated or contradicted pairings | Record exclusion reason; do not promote into benchmark candidates. |

**Ranking within tiers:** first target-trade relevance and evidenced US location, then strength of pairing/revision evidence, quantity-to-geometry traceability, readable/calibratable inputs, independent review, and clarity of permitted use. Prioritize A over B; C/D should not inflate the reported count of paired packages. Rights uncertainty is a hold on reuse/publication, not proof that the artifact does not exist.

**Hold for investigation:** unknown US jurisdiction, inaccessible downloads, unclear phase/revision, conflicting title blocks, incomplete sheets, uncertain permissions, or quantities that cannot be assigned to a scope. A rejection of a claimed pairing need not discard individually useful input assets.

### Project identity and document matching

- Establish US location from a project address, city/state, issuing US agency or explicit project description; record the precise page/section and evidence. A US vendor address, English text or imperial units alone do not establish project jurisdiction.
- Compare project title/number, location, sheet IDs, issue dates, revision/addendum numbers, phase, rooms, trade and geometry. Preserve discrepancies. Filenames and co-location on a samples page are only weak evidence.
- Record which assets support each pairing, the evidence locator, verification method and confidence (`verified`, `probable`, `unresolved`, `contradicted`). Never silently combine projects, design phases, bid alternates or revisions.
- Preserve revision history and superseded documents. Map addenda to affected sheets and quantities; do not assume the newest file is the quantity report's source.
- Record missing assets as missing. Do not invent a specification, clean drawing or relationship to make a package appear complete.

### Original drawings versus removable overlays

Use `verified_original`, `unmarked_provenance_unverified`, `marked_only`, or `derived_overlay_removed` as distinct statuses. A PDF with removable annotation layers is a **possible recovery route**, not verified original evidence. If removal is permitted and performed later, retain the source, document the transformation and compare underlying geometry/text; flattened marks may obscure original content. Never describe an edited reconstruction as an original drawing. Detect answer leakage in input layers, hidden annotations, attachments and embedded takeoff tables.

## Answer quality and review

Keep a vendor's sample, instructional worked solution, estimator-produced takeoff and independently checked reference distinct. Record authoring organization, stated purpose, public reviewer attribution where relevant, review date and actual verification performed. Avoid collecting unnecessary personal information.

Use answer status `unreviewed_example`, `reviewed_with_issues`, or `expert_verified_reference`; reserve the last for a documented independent trade review, reproducible rules and resolved material discrepancies. Marketing language is not correctness evidence.

Where possible, each quantity line should trace to **asset → PDF page index and printed sheet ID → floor/room/zone → assembly/finish → markup ID or geometry**. Store PDF page index as 1-based, separately from the printed label. Record worksheet/cell range or report page/row for quantities. Capture coordinate system, origin, rotation, page dimensions, scale by viewport and calibration reference when geometry is available. A title-block scale alone may be invalid after resizing.

Preserve gross/net methods, opening thresholds, wall height sources, sides/layers, coat assumptions, waste/rounding, alternate scope and exclusions. Do not infer absent rules as fact. Keep alternative valid decompositions (for example by room versus wall type) and equivalence mappings rather than forcing one canonical itemization. Document ambiguities, acceptable tolerances and unresolved disagreements; use geometry, scope and aggregate reconciliation together. Group duplicate projects and revisions before any train/evaluation split to prevent leakage.

## Source evidence and provenance

A useful research record connects the source landing page to actual downloadable files and distinguishes verified content from publisher claims and inference. Search snippets, previews and download labels alone do not establish that a usable document is available.

The supporting metadata includes original and resolved public URLs, date checked, access result, file format, page count, readability and SHA-256 hash where a file has been retrieved. Public records exclude credentials, session tokens and signed-link secrets. Exact duplicates and likely related versions are identified separately. Missing roles, conflicting metadata, review status and rights uncertainty remain visible in the record.

### Source classes

- Estimating firms' trade-specific sample packages: promising answer evidence, often incomplete inputs and unclear reuse rights.
- Estimating software training and university construction-management exercises: potentially paired worked examples; check that downloads are available and that answers correspond to the supplied exercise.
- Public procurement, school districts, municipalities, universities and other public owners: strong potential for drawings, specifications and addenda; bid tabulations are usually not detailed quantity answers.
- Academic supplements and repositories, GitHub, Hugging Face and Zenodo: check asset-level provenance, project country, task definition and license coverage. A repository license does not automatically cover third-party drawings.
- Trade associations and public instructional resources: useful measurement rules and worked examples; distinguish generic teaching diagrams from real project packages.

### Illustrative research queries

The following query templates cover the priority trades and source classes. Braced terms represent a project, city or state of interest.

```text
"drywall" "sample takeoff" "drawings" filetype:pdf
"metal stud" "quantity takeoff" "sample" (xlsx OR pdf)
"painting" "takeoff" "marked plans" "sample"
"drywall" "worked example" "plans" site:edu
"{project name}" ("specifications" OR "addendum" OR "finish schedule")
"{city state}" "bid documents" ("gypsum board" OR "painting")
site:gov "{state}" "09 29 00" "drawings"
site:edu "09 91 00" "project manual"
site:github.com "quantity takeoff" (drywall OR painting)
site:huggingface.co/datasets "construction drawings"
site:zenodo.org "quantity takeoff"
```

These queries do not imply that a complete package exists. Related terminology includes gypsum board/GWB, partitions, cold-formed metal framing, finishes, coating and reflected ceiling plan. Drywall/framing and painting remain the primary research scope.

## Access, permissions and licensing

Source use is subject to site terms, robots policies, rate limits and access restrictions. Only permitted access is in scope; login or paywall bypass, CAPTCHA circumvention, access-control evasion and credential harvesting are excluded. Unavailable access is recorded as `access_restricted`.

**Publicly accessible is not the same as licensed for redistribution or model training.** Record asset-level license text/URL, terms URL, attribution requirements, permission evidence and unknowns. Distinguish access permission, local research use, redistribution and training permission; use `unknown` when unsupported. Do not infer public-domain status merely from a government host. Keep restricted or unresolved files out of a public collection until the intended use is authorized. This brief grants no rights in third-party materials.

## Research record schema

The desired research record consists of a package manifest (JSON or JSONL), an asset inventory and a concise assessment of evidence and missing assets. Raw source facts remain alongside normalized values. Unknown values use `null` with an explanation.

| Group | Required fields |
|---|---|
| Record | `schema_version`, `package_id`, `discovered_at`, `checked_at`, `source_class`, `search_query`, `landing_page_url` |
| Project | `project_name`, `project_number`, `building_type`, `location` (country/state/city/address as available), `us_evidence` (asset/URL, page/section, factual excerpt), `trade`, `scope`, `phase`, `revision`, `issue_date`, `addenda` |
| Asset | `asset_id`, `role`, `original_url`, `download_url`, `filename`, `sha256`, `format`, `mime_type`, `byte_size`, `page_count`, `sheet_ids`, `page_scope`, `retrieved_at`, `http_status`, `download_status`, `original_status` |
| Measurement | `units`, `quantity_basis`, `measurement_rules`, `calibration`, `layers`, `quantity_locators`, `geometry_links`, `assumptions`, `exclusions`, `alternates` |
| Pairing | `related_asset_ids`, `pairing_evidence` (claim, evidence locator, method, confidence), `revision_conflicts`, `missing_assets` (role, reason, search attempted) |
| Assessment | `package_tier`, `answer_status`, `quality_flags`, `review_provenance`, `ambiguities`, `alternative_decompositions`, `priority`, `disposition`, `rejection_reason` |
| Rights/access | `access_status`, `terms_url`, `license_name`, `license_url`, `license_evidence`, `allowed_uses` (research/redistribution/training separately), `permission_status`, `attribution`, `restrictions` |

Roles: `original_drawing`, `specification`, `marked_drawing`, `quantity_takeoff`, `schedule`, `addendum`, `rfi`, `measurement_metadata`, `assumptions_exclusions`. One file may have multiple roles; identify the relevant pages rather than duplicating bytes. Mark extracted/normalized files as derivatives and link their source hashes.

### Hypothetical manifest fragment — not a real source or benchmark

The reserved `example.invalid` URLs and all identifiers below are illustrative. This shortened fragment shows how uncertainty should be represented; complete research records include the fields above.

```json
{
  "schema_version": "1.0",
  "package_id": "hypothetical-interiors-001",
  "project_name": "HYPOTHETICAL commercial interiors",
  "location": {"country": null, "state": null, "city": null},
  "us_evidence": [],
  "trade": ["drywall_framing"],
  "phase": null,
  "revision": null,
  "landing_page_url": "https://example.invalid/sample",
  "assets": [{
    "asset_id": "hypothetical-quantity-file",
    "role": ["quantity_takeoff"],
    "original_url": "https://example.invalid/sample/takeoff.xlsx",
    "download_url": null,
    "filename": "hypothetical-takeoff.xlsx",
    "format": "xlsx",
    "sha256": null,
    "page_count": null,
    "page_scope": null,
    "scope": "publisher claims drywall; unverified",
    "units": [],
    "download_status": "not_retrieved",
    "original_status": null
  }],
  "pairing_evidence": [],
  "missing_assets": [
    {"role": "original_drawing", "reason": "not located"},
    {"role": "specification", "reason": "not located"},
    {"role": "marked_drawing", "reason": "not located"}
  ],
  "package_tier": "C",
  "answer_status": "unreviewed_example",
  "quality_flags": ["US location unresolved", "file not inspected"],
  "access_status": "unverified",
  "license_name": null,
  "allowed_uses": {"research": "unknown", "redistribution": "unknown", "training": "unknown"},
  "disposition": "hold"
}
```

## Suggested research archive structure

```text
collection/
  manifest.jsonl
  asset_inventory.csv
  review_report.md
  rejected_or_held.jsonl
  packages/<package_id>/
    metadata.json
    pairing_evidence.json
    missing_assets.json
    inputs/                 # permitted original drawings and specifications
    answers/                # permitted marked drawings and quantity reports
    supporting/             # schedules, addenda, RFIs and rules
    derived/                # labeled extracts/conversions; never called originals
```

Retained files are limited to assets with appropriate permission. Records with blocked access or unresolved retention rights contain metadata and links only. An accompanying report summarizes A/B/C/D packages separately, US and pairing evidence, rights holds, duplicates, review gaps and missing assets. The research objective is useful, traceable paired evidence.

## Public examples

### Lead example: Dover High School / Career Technical Center

**Dover is the lead example of the evidence structure described in this brief.** [Caliper's public sample page](https://calipertakeoffs.com/) links a [framing, drywall and ceilings quantity PDF](https://calipertakeoffs.com/samples/caliper-sample-framing-drywall.pdf) and a [public marked drawing preview](https://calipertakeoffs.com/samples/markup-framing-drywall.webp). Both files were successfully retrieved on October 10, 2026. The one-page quantity PDF identifies **25 Alumni Drive, Dover, New Hampshire**, establishing US project location, and describes a portfolio exercise rather than commissioned client work.

The PDF names the **100% Conformed Set dated September 12, 2016**, with Second Floor Plan **A2.2C**, Second Floor RCP **A3.2C**, and Partition Types **A8.1**, scoped to **Second Floor — Part C**. It includes quantity categories for partitions, framing-related scope and ceilings, plus measurement assumptions and exclusions. Its value as an example comes from a named US project, identified source sheets/revision, marked geometry and a quantity summary whose basis can be investigated.

The [City of Dover project index](https://www.dover.nh.gov/government/city-operations/public-education/high-school-project/index.html) publishes the conformed construction drawings and specifications. Relevant official input documents include:

- [Specifications, Volume 1](https://www.dover.nh.gov/Assets/government/city-operations/public-education/high-school-project/drawings-specs/Specifications%20-%20VOL%201%20-DHS%20Conformed%20Set.pdf).
- [Drawings, Volume 1 of 4, Part 2](https://www.dover.nh.gov/Assets/government/city-operations/public-education/high-school-project/drawings-specs/Vol%201%20of%204%20DHS-CTC-Conformed%20Set_Part2.pdf).
- [Drawings, Volume 1 of 4, Part 3](https://www.dover.nh.gov/Assets/government/city-operations/public-education/high-school-project/drawings-specs/Vol%201%20of%204%20DHS-CTC-Conformed%20Set_Part3.pdf).

Verification on October 10, 2026: all five linked input/output assets returned HTTP 200 without credentials. The cropped raster markup was visually paired with clean **A2.2C (Part 2, PDF page 14)**. **A3.2C is Part 2, PDF page 42**; **A8.1 is Part 3, PDF page 16**; **specification section 092900 starts at Volume 1, PDF page 697**. Page numbers here are 1-based physical PDF pages. The quantity summary explicitly cites the same conformed-set date and sheet IDs. The markup crop has no title block, so retain the visual pairing evidence alongside the vendor's explicit source citation.

**Current status: partial public-source worked example, unreviewed vendor output.** This joins official input-document sources to a vendor quantity summary and marked preview. It meets Tier B for the evidenced partial scope, with further scope reconciliation required before benchmark use. The public quantity PDF is a one-page summary, not a verified downloadable Excel workbook: references to workbook tabs or deliverables do not establish that those files are public. The separate markup is a preview image, not a verified complete marked PDF. Detailed takeoff tabs, ceiling markup and independent correctness review remain missing. Preserve asset-level pairing evidence before promoting any scope to an accepted benchmark. Public access does not establish redistribution or training permission; the drawings carry HMFH copyright and the sample carries Caliper copyright, with no redistribution license found. Quantities have not been independently validated. This is a drywall/framing/ceiling exemplar, not a verified painting answer package.

### Additional trade-specific examples

Checked October 10, 2026: the four PDF links below returned HTTP 200 and their contents were inspected. These are **Tier C marketing examples, not gold references**. No complete clean-drawings + specifications + marked-drawings + quantity package was established in this bounded check. Download availability can change; recheck before collection. Reuse, redistribution and training permissions are unknown; the sites display all-rights-reserved notices.

| Example and landing page | Direct downloadable file | Observed evidence | Gaps and unresolved evidence |
|---|---|---|---|
| [Kapolei commercial drywall sample](https://drywalltakeoffservices.us/drywall-estimate-sample/) | [12-page drywall/framing PDF](https://drywalltakeoffservices.us/wp-content/uploads/2026/07/drywall-takeoff-sample-commercial_-Hawai.pdf) | Gypsum board, metal studs and track quantities; color-coded marked floor/locker drawings. Quantity cover and marked sheet A201 identify U-Haul Moving & Storage of Kapolei, Building A, Kapolei, HI 96707: US location evidenced. | Separate clean drawings and specifications not verified. A201 shows December 18, 2024 bid/permit and May 8, 2025 plan-check revisions; takeoff date is blank, so revision alignment remains unverified. Seek the matching issued originals/specifications and confirm quantity basis. |
| Veracity exterior/interior drywall example; discovery URL is the PDF itself (separate landing page not verified) | [6-page drywall PDF](https://veracityestimating.com/wp-content/uploads/2025/02/exterior-and-interior-finishes-drywall-estimate-sample.pdf) | Quantities, costs and marked overlays; project/location redacted. | US project location unknown. Clean drawings, specifications and revision alignment not verified; hold for identity and pairing evidence. |
| [Commercial painting samples](https://paintingtakeoffservices.com/painting-estimate-samples/) | [16-page commercial painting PDF](https://paintingtakeoffservices.com/wp-content/uploads/2025/02/commercial-painting-takeoff-sample.pdf) | Walmart-branded scope, interior/exterior quantities and color-coded architectural/MEP marks. | Location blank/redacted; US location unverified. Brand and units do not establish jurisdiction. Separate clean plans, specifications and revision alignment not verified. |
| [Hotel painting sample landing page](https://paintingtakeoffservices.com/painting-estimate-samples/) | [23-page hotel painting PDF](https://paintingtakeoffservices.com/wp-content/uploads/2025/02/commercial-painting-takeoff-sample-hotel.pdf) | Room/wall/ceiling quantities, room counts and measured architectural drawings. | US project location unverified: an architect's Charlotte, NC address is not a project address. Clean plans, specifications and revision alignment not verified. |

These examples illustrate partial evidence records. Missing matching assets, redacted information and unresolved correctness remain explicit limitations; presentation quality alone does not establish reference quality.
