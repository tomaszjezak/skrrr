# skrrr — US drywall and framing benchmark-data research brief

## Purpose

Find new, retrievable US construction packages that can support serious drywall and framing quantity-takeoff benchmarks. This document is the complete research brief: use the requirements, existing-source register and reporting format below without assuming any other context.

**Unmarked source drawings + matching specifications and scope context → matched marked drawings or native measurable geometry + actual multi-row takeoff quantities.**

The primary scope is US commercial interiors: offices, schools, healthcare, retail, hospitality, multifamily and tenant improvements. Prioritize gypsum-board assemblies and light-gauge metal framing, including associated ceilings, soffits, shaft walls and insulation. Identify wood framing separately; do not pass a timber-joist example off as a drywall/metal-stud package. The unit of analysis is a **project × trade × bounded sheet/floor/area scope × phase × revision package**.

The desired result is a usable project package with many meaningful reference rows and measurements, not a list of promising websites or isolated one-quantity exercises. Prefer complete trade packages spanning several assemblies, rooms, floors or sheets. A genuinely complete smaller scope can be valuable, but one room, one polygon or one total is a limited diagnostic, not success against this brief. Do not split a single quantity into artificial rows to make it look substantial.

This repository must remain **exactly one Markdown file**. It contains the research brief and the already-found register only. Any collected files, manifests and research reports belong in the separately authorized research destination, not as additional repository files. Do not place private company-provided material, private links, credentials or internal evaluation artifacts in this public brief.

## Evidence requirements

| Role | Required for an ideal package | Details |
|---|---|---|
| Input | Original, unmarked drawings | Architectural plans, reflected ceiling plans, elevations, sections, details, relevant schedules and sheet index; readable dimensions and scale. |
| Input | Matching specifications and controlling context | Project-specific trade sections, wall/partition schedules, details, relevant room/finish schedules and applicable general requirements. Include addenda and RFI answers when they affect the measured scope. Embedded drawing notes may suffice for a bounded scope only with an explicit sufficiency assessment; do not invent a missing manual. |
| Answer evidence | Marked-up drawings or native measurable markup geometry | Measured lines, polygons, cutouts, counts, legends and labels tied to the same sheets and revision. Prefer the actual marked PDF plus editable annotation export or native project. A native project must yield inspectable geometry, sheet bindings and quantity values; possession of an installer alone is insufficient. |
| Answer evidence | Actual multi-row completed takeoff | XLS/XLSX/CSV or native quantity export preferred; readable quantity-report PDF or explicit native measurement records also acceptable. Require original numerical values, descriptions/material or assembly mapping, units, scope breakdown and traceability to geometry. Report missing mapping honestly. A blank template, price-only bid, one total, screenshot or promise of an unavailable workbook is insufficient. |
| Supporting | Required when it controls the measured scope | Applicable wall/finish/door schedules, addenda, RFI answers, assumptions/exclusions and measurement rules. Also retain scale calibration, annotation layers, software/version, review evidence and provenance. Do not demand unrelated project documents merely to inflate completeness. |
| Secondary | Optional commercial information | Labor, productivity, unit prices, waste, equipment and totals. Preserve separately from measured quantities; price evidence cannot replace quantity evidence. |

### Priority trades and quantity distinctions

1. **Drywall and associated metal framing:** partition types and lengths; wall heights; sides and board layers; board type/thickness; stud size, spacing/gauge, tracks and headers; shaft walls; ceilings, soffits and bulkheads; openings and returns; insulation and finish levels when in scope. Capture assembly definitions, not just a generic “drywall” label.
2. **Wood framing:** retain useful US joist, stud, beam, post and sheathing packages as a separately labeled framing category. State whether each value is a measured member length, assembly output, piece count or purchase quantity.
3. **Adjacent interior scope:** acoustical ceilings, insulation or finishes are useful where they explain the target assemblies. Painting is secondary and must be labeled separately; do not spend the main search effort on painting-only samples. Civil/sitework, structural concrete, roofing-only quantities and generic whole-building cost estimates do not count toward the requested drywall/framing yield.

Record units explicitly (SF, LF, EA, sheets, etc.), original precision and any conversions. Distinguish wall length, one-face area, two-face area, total board-layer area, ceiling horizontal projection, vertical returns, board count and purchase quantity. Never equate these without checking heights, sides, layers, opening deductions, waste, stock size, rounding and scope. Material/component output rows derived from the same assembly share geometry and are not independent measurements. Preserve painting-related coat and coverage conventions only when retaining a separate secondary painting record.

### Scope and size of the actual reference

For every candidate, give a precise answer to “What can be evaluated from the existing source answers?” Separate the extent of the **input documents**, **available source answers**, and **reviewed benchmark coverage**. A whole-building drawing set with six ceiling answers does not become a full-project answer key.

Record these counts, each with an evidence locator and counting rule:

- Clean and marked sheet counts; exact sheet IDs, PDF pages, floors, rooms/areas and viewports covered.
- Distinct relevant assembly types and source assembly instances, with material/height/side/layer definitions where supplied. Keep these two counts separate.
- All numerical quantity rows, relevant drywall rows, relevant metal-framing rows, relevant wood-framing rows, and other-trade rows. Separately count rows with missing units, derived component outputs, subtotals, and duplicate/repeated-floor report rows.
- Unique relevant source measurements by primitive: lines/segments, polylines, area polygons with cutouts, count groups and individual count markers. Also report source object counts when useful, without treating every object as a separate answer.
- Number of relevant quantity rows actually linked to geometry, number with verified source-sheet/revision alignment, and number reviewed for correctness. Give the denominator for each claim of coverage.

Use `null` and a reason for an unverified count; do not guess from page count or a photograph. One grouped count of 179 items is one quantity record and 179 markers, not 179 separate answers or 179 × 179 items. Repeated floors sharing a native plan are repeated scheduled scope, not new independent geometry. Exclude civil/roof/code-area measurements from drywall counts. Do not count totals and their component rows twice.

Prioritize multi-assembly, multi-row packages with substantial individual measurement coverage; use these evidenced counts to rank the results. Small diagnostic cases may remain in the register as useful history, but do not let a batch of one-number examples satisfy the objective.

## Package tiers and selection

Package completeness and answer correctness are separate axes. A complete vendor example is not automatically gold.

| Tier | Evidence available | Disposition |
|---|---|---|
| A — complete paired | Retrieved unmarked originals and adequate matching specifications/context, marked drawings or native measurable geometry, and meaningful multi-row quantities; same project/trade/scope/phase/revision evidenced | Highest priority for benchmark review; complete does not mean correct or licensed. |
| B — partial paired | Retrieved inputs and actual quantities have credible pairing, but specifications/context, marked geometry or reference coverage are partial | Retain with explicit gaps; qualify only the supported scope after review. |
| C — answer-side lead | Marked drawings and/or quantities; originals absent or pairing/revision unresolved | Discovery queue; do not claim a clean-input benchmark. |
| D — input-side lead | US drawings/specifications with no completed answers | Useful input inventory; independent takeoff creation would be a separate task. |
| Excluded | Unrelated trades, blank templates, cost-only summaries, unreadable artifacts, non-US projects, fabricated or contradicted pairings | Record exclusion reason; do not promote into benchmark candidates. |

**Ranking within tiers:** first target-trade relevance and evidenced US location, then strength of pairing/revision evidence, relevant assembly/row/measurement breadth, quantity-to-geometry traceability, readable/calibratable inputs, independent review, and clarity of permitted use. Prioritize A over B; C/D should not inflate the reported count of paired packages. Rights uncertainty is a hold on reuse/publication, not proof that the artifact does not exist.

**Hold for investigation:** unknown US jurisdiction, inaccessible downloads, unclear phase/revision, conflicting title blocks, incomplete sheets, uncertain permissions, or quantities that cannot be assigned to a scope. A rejection of a claimed pairing need not discard individually useful input assets.

### Readiness gates

Keep these stages explicit: **discovered lead → retrieved and inspected → qualified for benchmark review → admitted reference for a stated scope**. None of the tiers alone grants admission.

A candidate is qualified for review only when actual files have been retrieved and opened, the relevant multi-row scope is measurable from unmarked inputs, numerical reference values and geometry are inspectable, pairing/revisions are evidenced, and all material gaps/conflicts are documented. Admission additionally requires adjudicated scope and measurement rules, quantity/geometry reconciliation, an explicit coverage boundary, answer-quality review and permissions appropriate to the intended use.

An accepted partial reference must not pretend to cover the full assignment. Unreferenced model outputs are unscored, not automatically wrong; missing source reference coverage must not become a false-positive penalty. Quantity agreement with a source key and construction correctness are different claims. Do not manufacture an answer, alter an original source quantity, or silently reconcile a source defect to make admission possible.

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

Use answer status `unreviewed_example`, `source_agreement_reviewed`, `reviewed_with_issues`, or `expert_verified_reference`; reserve the last for a documented independent trade review, reproducible rules and resolved material discrepancies. Mechanical checks, visual checks and assistant reviews must be described as what they are; they do not establish professional-estimator certification. Marketing language is not correctness evidence.

Where possible, each quantity line should trace to **asset → PDF page index and printed sheet ID → floor/room/zone → assembly/finish → markup ID or geometry**. Store PDF page index as 1-based, separately from the printed label. Record worksheet/cell range or report page/row for quantities. Capture coordinate system, origin, rotation, page dimensions, scale by viewport and calibration reference when geometry is available. A title-block scale alone may be invalid after resizing.

Preserve gross/net methods, opening thresholds, wall height sources, sides/layers, coat assumptions, waste/rounding, alternate scope and exclusions. Do not infer absent rules as fact. Keep alternative valid decompositions (for example by room versus wall type) and equivalence mappings rather than forcing one canonical itemization. Document ambiguities, acceptable tolerances and unresolved disagreements; use geometry, scope and aggregate reconciliation together. Group duplicate projects and revisions before any train/evaluation split to prevent leakage.

## Source evidence and provenance

A useful research record connects the source landing page to **actual retrievable files** and distinguishes verified content from publisher claims and inference. Search snippets, previews, photographs, screenshots and download labels alone do not establish that a usable package is available.

Open and inspect the actual PDF, workbook, archive or native project. Check file signatures, workbook tabs and rows, PDF page content, archive member names and readable quantities. An HTTP 200 that returns a login page, HTML error or empty file is not a successful file retrieval. Record the stable publisher link and resolved destination; never publish expiring signed URLs or session secrets. A portal is a discovery/access route until its actual attachments are obtained. For native jobs, inventory relevant source drawings, geometry, quantities, units and software/version without claiming that an installer is itself a project answer. Use safe inspection/extraction; installation or execution requires the applicable authorization.

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
"drywall" "framing" "marked plans" (xls OR xlsx OR zip)
"drywall" "worked example" "plans" site:edu
"{project name}" ("specifications" OR "addendum" OR "finish schedule")
"{city state}" "bid documents" ("gypsum board" OR "metal framing")
site:gov "{state}" "09 29 00" "drawings"
site:edu "09 22 16" "project manual"
site:github.com "quantity takeoff" (drywall OR framing)
site:huggingface.co/datasets "construction drawings"
site:zenodo.org "quantity takeoff"
```

These queries do not imply that a complete package exists. Related terminology includes gypsum board/GWB, partitions, cold-formed metal framing, metal studs, light-gauge framing, partition schedules, reflected ceiling plans, takeoff reports, PlanSwift, On-Screen Takeoff/OST, Bluebeam annotations and estimating answer keys.

### Research sequence and continuation

1. Read **Already found** first. Deduplicate by project identity, original file hashes and revision, not just URL or vendor branding. A mirror, renamed ZIP, extra screenshot or re-export of an existing package is not a new project.
2. Pursue two explicit tracks: genuinely new paired project packages, and missing-file/revision/scope gaps in known packages. Label each result `new_project` or `known_project_gap_filled`; merely finding an old URL again is neither.
3. Start with sources likely to provide both answers and inputs: native sample jobs, university worked exercises/competition answers and complete estimator sample bundles. Pair their actual files with official owner/design-team drawing/specification archives only when project and revision evidence supports it.
4. For a promising known project, search its exact title, number, address, sheet IDs, issue dates and architect/owner together with specifications, addenda, schedules and takeoff terms. Follow relevant source-page links and archive inventories. Do not join unrelated projects just because their plan layouts look similar.
5. Inspect before promoting. Follow the readiness gates and retain evidence of failures. Where a site is blocked, try another permitted public source or archive of the same identified document; never evade access controls. State what could not be checked.
6. Continue across source classes rather than stopping at the first plausible PDF or spending the whole search on a blocked source. Prioritize the expected gain in usable drywall/framing coverage. Checkpoint inspected findings and unresolved gaps during long research so progress survives interruption.
7. End with retrieved evidence and an honest status for each candidate. It is valid to find no new qualifying package. Do not pad the outcome with unrelated trades, already-known duplicates, fabricated answers or uninspected leads.

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
| Scope/counts | `input_scope`, `answer_scope`, `reviewed_scope`, `clean_sheet_count`, `marked_sheet_count`, `assembly_type_count`, `assembly_instance_count`, `relevant_row_counts_by_trade`, `rows_with_units`, `duplicate_row_count`, `measurement_counts_by_primitive`, `quantity_geometry_linked_rows`, `count_evidence` |
| Measurement | `units`, `quantity_basis`, `measurement_rules`, `calibration`, `layers`, `quantity_locators`, `geometry_links`, `assumptions`, `exclusions`, `alternates` |
| Pairing | `related_asset_ids`, `pairing_evidence` (claim, evidence locator, method, confidence), `revision_conflicts`, `missing_assets` (role, reason, search attempted) |
| Assessment | `package_tier`, `readiness_stage`, `novelty_status`, `answer_status`, `quality_flags`, `review_provenance`, `ambiguities`, `alternative_decompositions`, `priority`, `disposition`, `rejection_reason` |
| Rights/access | `access_status`, `terms_url`, `license_name`, `license_url`, `license_evidence`, `allowed_uses` (research/redistribution/training separately), `permission_status`, `attribution`, `restrictions` |

Roles: `original_drawing`, `specification`, `marked_drawing`, `quantity_takeoff`, `schedule`, `addendum`, `rfi`, `measurement_metadata`, `assumptions_exclusions`. One file may have multiple roles; identify the relevant pages rather than duplicating bytes. Mark extracted/normalized files as derivatives and link their source hashes.

### Required research report

Lead with the best usable findings, then the gaps. Report:

1. **New qualifying packages:** exact project/trade/scope; status and reason; direct source-file links and retrieval/inspection date; assembly, relevant-row and measurement counts; pairing/revision evidence; rights and review limits.
2. **Known-project improvements:** the exact new asset or gap resolved, linked back to the existing project. Explain what coverage changed and what is still missing.
3. **Held or rejected candidates:** links, actual evidence, blocker/rejection reason and the most useful next retrieval step. Keep mere leads separate from inspected files.
4. **Coverage summary:** unique new projects, qualified scopes, relevant rows/measurements and unresolved cases, with duplicates and secondary trades separated. Never add incompatible units into a single quantity total.
5. **Retrieval handoff:** an asset manifest, original files where retention is permitted, source hashes, native/quantity extracts clearly labeled as derivatives, and precise missing-file requests. A prose report with inaccessible landing pages is not a complete delivery.

Each project entry must be self-contained enough for another reviewer to retrieve the sources and reproduce the claimed counts and pairings. Preserve exact original source values before normalization. Name any transform used to recover clean drawings, convert units or extract geometry. Do not include private company records or evaluator-only artifacts in a public report.

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

## Already found

This register prevents repeated discovery and directs effort toward new projects and concrete gaps. It is an inventory of **public sources and their limitations**, not a declaration that every source is benchmark-ready. Historical verification dates are stated below; recheck links when retrieving. Counts describe source content, not automatically correct, independent or admitted answers. Source rows, deduplicated rows, measurement objects and benchmark scoring groups are different populations; this register does not define a current evaluation denominator. Rights for redistribution/model training remain unestablished unless explicitly evidenced.

### Known project packages

#### Monroe / 713–715 Monroe Street, Hoboken, New Jersey

- Sources: [Simsona finishes sample page](https://www.simsona.com/finishesestimating/) and [Monroe source ZIP](https://www.simsona.com/wp-content/uploads/2025/02/Monroe.zip), retrieved and reviewed October 10, 2026.
- Found: native PlanSwift project, marked drawings, XLS takeoff and PDF report; five clean source TIFF sheets recoverable from the native archive. Clean-PDF conversions are derivatives, not separately published originals. Sheets: A02.00, A02.01, A02.02, S-3 and S-4.
- Scope/size: 13 explicit-unit drywall rows and 5 metal-framing rows; 10 and 4 respectively after collapsing repeated-floor copies. Two additional drywall roof rows lack units. Wood framing and other trades are also present and must be counted separately. The native drywall/material lineage includes 34 wall-assembly parents; shared floor geometry and derived component rows must not inflate independent-example counts.
- Status: **known partial paired/source-agreement package, not a complete certified drywall/framing reference**. Board/stud rows are material EA outputs, not direct wall SF/LF. The supplied clean sheets do not establish all wall heights/types and layer conventions; no standalone specification manual or complete wall-type/detail schedule was supplied. Source formula, rounding, labeling and repeated-floor conflicts require explicit review.
- Seek: the matching public wall schedules/details/specifications and issue history; evidence resolving assembly/height/layer conventions and source discrepancies. More copies of the same ZIP or the single roof-joist diagnostic do not count as new project coverage.

#### ASC Region 7, 2018 Residential/Multi-Family / 710 Wilshire mock-up, Santa Monica, California

- Sources: [original 18-page mock-up](https://asc67.org/ASC_Previous_Problems/R7/Residential_MultiFamily/2018/Mockup.pdf), [marked answer mock-up](https://asc67.org/ASC_Previous_Problems/R7/Residential_MultiFamily/2018/Section%20IV%20-%20Estimating%20-%20Answers/Mockup.pdf), [ASC estimate workbook](https://asc67.org/ASC_Previous_Problems/R7/Residential_MultiFamily/2018/Section%20IV%20-%20Estimating%20-%20Answers/ASC%20Estimate.xlsx) and [full-project specifications, Volume 1](https://asc67.org/ASC_Previous_Problems/R7/Residential_MultiFamily/2018/Specs/Specifications/710%20Wilshire%20-%20Addendum%2005%20Specifications%20Vol%201.pdf), retrieved and reviewed October 10, 2026.
- Found: genuine clean/marked mock-up pair, completed multi-trade workbook and native measured geometry. Relevant evidence includes rated/non-rated wall lines on A-111 and gypsum ceiling polygons on A-121. The workbook is broader than drywall; its full row count must not be reported as drywall reference breadth.
- Status: **known partial paired worked example with source discrepancies and limited scope**. The mock-up refers to Addendum 06 while the supplied full-project specifications are Addendum 05. Full-hotel documents do not supply full-hotel takeoff answers. Wall-line/quantity rounding and the non-rated wall discrepancy require reconciliation; board/stud procurement references must not be manufactured from area/length formulas.
- Seek: exact matching mock-up specifications and referenced wall/ceiling details, documented source conventions, and any genuinely additional native drywall/framing answers. Keep unrelated concrete, rebar and MEP workbook entries out of target-trade counts.

#### Positive Tomorrows Elementary School, Oklahoma City, Oklahoma

- Sources: [144-page drawing PDF](https://canvas.ou.edu/courses/365351/files/108682784/download?download_frd=1) and [1,022-page specification PDF](https://canvas.ou.edu/courses/365351/files/108682811/download?download_frd=1), publicly retrieved without authentication and reviewed October 10, 2026. Use these stable source links rather than copying transient CDN redirects.
- Found: project 2813E06 drawings/specifications, editable native measurements, ceiling plan A121A (physical PDF page 53), schedules and relevant gypsum/framing specifications. The drawing source is marked; clean copies made by removing verified measurement overlays are **derived_overlay_removed**, not independently obtained originals.
- Scope/size: 83 logical native measurement records across mixed trades, including 20 ceiling-area records on A121A. The full file has 261 measurement objects, including 179 markers belonging to one grouped count. These totals are not drywall answer counts. Civil, roof, code-area and floor-finish measurements must be excluded from drywall reference breadth; overlapping, mixed-material and zero-area ceiling marks need review.
- Status: **known partial native-geometry reference, incomplete for whole-project drywall/framing**. No complete original wall/framing quantity schedule was established. Drawings are dated February 26, 2018 and the specification cover March 2018; exact revision equivalence/addenda completeness remain unresolved. Clean-input recovery, source-category mapping and limited answer coverage must stay explicit.
- Seek: separately published unmarked originals of the same issue, completed wall/framing quantities, matching revision/addendum context, and further source-backed ceiling records. Do not present a one-room diagnostic or the broad overlapping ceiling polygon as a full-project takeoff.

#### Dover High School / Career Technical Center, Dover, New Hampshire

**Dover is a known partial example, useful for closing specific gaps.** [Caliper's public sample page](https://calipertakeoffs.com/) links a [framing, drywall and ceilings quantity PDF](https://calipertakeoffs.com/samples/caliper-sample-framing-drywall.pdf) and a [public marked drawing preview](https://calipertakeoffs.com/samples/markup-framing-drywall.webp). Both files were successfully retrieved on October 10, 2026. The one-page quantity PDF identifies **25 Alumni Drive, Dover, New Hampshire**, establishing US project location, and describes a portfolio exercise rather than commissioned client work.

The PDF names the **100% Conformed Set dated September 12, 2016**, with Second Floor Plan **A2.2C**, Second Floor RCP **A3.2C**, and Partition Types **A8.1**, scoped to **Second Floor — Part C**. It includes quantity categories for partitions, framing-related scope and ceilings, plus measurement assumptions and exclusions. Its value as an example comes from a named US project, identified source sheets/revision, marked geometry and a quantity summary whose basis can be investigated.

The [City of Dover project index](https://www.dover.nh.gov/government/city-operations/public-education/high-school-project/index.html) publishes the conformed construction drawings and specifications. Relevant official input documents include:

- [Specifications, Volume 1](https://www.dover.nh.gov/Assets/government/city-operations/public-education/high-school-project/drawings-specs/Specifications%20-%20VOL%201%20-DHS%20Conformed%20Set.pdf).
- [Drawings, Volume 1 of 4, Part 2](https://www.dover.nh.gov/Assets/government/city-operations/public-education/high-school-project/drawings-specs/Vol%201%20of%204%20DHS-CTC-Conformed%20Set_Part2.pdf).
- [Drawings, Volume 1 of 4, Part 3](https://www.dover.nh.gov/Assets/government/city-operations/public-education/high-school-project/drawings-specs/Vol%201%20of%204%20DHS-CTC-Conformed%20Set_Part3.pdf).

Verification on October 10, 2026: all five linked input/output assets returned HTTP 200 without credentials. The cropped raster markup was visually paired with clean **A2.2C (Part 2, PDF page 14)**. **A3.2C is Part 2, PDF page 42**; **A8.1 is Part 3, PDF page 16**; **specification section 092900 starts at Volume 1, PDF page 697**. Page numbers here are 1-based physical PDF pages. The quantity summary explicitly cites the same conformed-set date and sheet IDs. The markup crop has no title block, so retain the visual pairing evidence alongside the vendor's explicit source citation.

**Current status: partial public-source worked example, unreviewed vendor output.** This joins official input-document sources to a vendor quantity summary and marked preview. It meets Tier B for the evidenced partial scope, with further scope reconciliation required before benchmark use. The public quantity PDF is a one-page summary, not a verified downloadable Excel workbook: references to workbook tabs or deliverables do not establish that those files are public. The separate markup is a preview image, not a verified complete marked PDF. Detailed takeoff tabs, ceiling markup and independent correctness review remain missing. Preserve asset-level pairing evidence before promoting any scope to an accepted benchmark. Public access does not establish redistribution or training permission; the drawings carry HMFH copyright and the sample carries Caliper copyright, with no redistribution license found. Quantities have not been independently validated. This is a drywall/framing/ceiling exemplar, not a verified painting answer package.

### Newly inspected leads to continue, not admitted references

The following source assets were retrieved on **October 11, 2026 (UTC)**. Their actual content is more informative than the discovery photograph, but none is promoted to an admitted benchmark package here. Focus on the stated gaps rather than rediscovering these URLs.

#### University of Florida Rinker Hall

- Inputs: [A103 drawing](https://coremng.dcp.ufl.edu/rinkerhall/images/rinker/Drawings/Rinker_010.pdf), [A701 partition-type drawing](https://coremng.dcp.ufl.edu/rinkerhall/images/rinker/Drawings/Rinker_037.pdf), [A152 second/third-floor reflected ceiling plan (height context)](https://coremng.dcp.ufl.edu/rinkerhall/images/rinker/Drawings/Rinker_015.pdf) and [Division 9 specifications](https://coremng.dcp.ufl.edu/rinkerhall/images/rinker/specs/09_Finishes.pdf). Publisher indexes: [drawings](https://coremng.dcp.ufl.edu/rinkerhall/drawings.htm) and [specifications](https://coremng.dcp.ufl.edu/rinkerhall/specif.htm).
- Answer-side source: [Garcia thesis PDF](https://ufdcimages.uflib.ufl.edu/UF/E0/04/45/86/00001/GARCIA_C.pdf), with [university catalog record](https://ufdc.ufl.edu/UFE0044586/00001).
- Verified content: **65 baseline room/partition takeoff rows on physical PDF pages 98–100**, not just pages 98–99. The thesis states a third-floor-only scope on page 52. The marked figure on page 67 is raster imagery at 1024 × 464 resolution, not native measurement geometry.
- Status: **retrieved partial paired research lead**. The multi-row baseline is promising, but a small raster figure does not establish precise row-to-geometry alignment, complete measurable reference coverage or construction correctness. Keep baseline and proposed/alternative quantities separate.
- Seek: full-resolution marked plans or native takeoff files, explicit row/partition-to-sheet geometry mapping, baseline assembly/units and exact source-issue alignment. The drawing index reserves reproduction/transmission rights; do not redistribute the source assets without appropriate permission.

#### Burgundy Farm Community Arts

- Sources: [author's final-report page](https://mxf5229.wixsite.com/aethesis/final-report) and [actual final-report PDF](https://db92efea-d2a4-43f3-906f-4b5651912302.filesusr.com/ugd/9dfae5_aed6549c13b44e0aa3be7bc9531fd266.pdf).
- Verified content: **58 proposed exterior prefabricated light-gauge metal-framing/sheathing panel rows** on physical PDF page 71: 13 lower-level, 33 main-level and 12 mezzanine rows. The report contains clean lower/main plan reproductions on pages 49–50 and matching A1.1/A1.2 marked layouts on pages 68–69, plus a mezzanine marked layout on page 70. Native annotations are present: 13 panel polygons/square shapes on page 68, 33 polygons on page 69 and 12 rectangles on page 70, with associated line annotations. These are retrievable native panel shapes, not merely screenshot marks.
- Status: **retrieved partial paired panelization study, not a complete drywall takeoff**. Panel rows describe a proposed prefabrication design. The row-number-to-marked-segment mapping is inferred rather than explicitly keyed; unlabeled colors and dimensions do not resolve that mapping. Plans identify Bulletin 2 dated February 27, 2017, while assembly SK12 is dated April 11, 2017; applicability/revision alignment needs verification.
- Seek: original-resolution issued plans including matching clean mezzanine scope, an explicit numbered panel schedule-to-native-shape map, verified annotation calibration/measurement semantics, controlling assembly specifications and revision/addendum context. Do not present the 58 panel rows as 58 verified drywall assemblies or independent correct answers.

#### Crowne at Buck Island, Building 3

- Sources: [vendor portfolio](https://solidtakeoffs.com/portfolio/), [marked takeoff PDF](https://solidtakeoffs.com/wp-content/uploads/2026/09/CROWN-AT-BUCK-ISLAND-BUILDING3-TAKEOFF.pdf) and [actual BOQ workbook](https://solidtakeoffs.com/wp-content/uploads/2026/09/CROWN-AT-BUCK-ISLAND-BUILDING3-BOQ.xlsx).
- Input-discovery routes: [Town of Bluffton plan attachments](https://townofblufftonsc-energovweb.tylerhost.net/apps/selfservice#/plan/96acbb53-1d4d-4045-b508-666974059608?tab=attachments) and [permit record](https://townofblufftonsc-energovweb.tylerhost.net/apps/selfservice#/permit/52fb5d51-40ca-4adc-ad0a-6605006e9829). The 25-page clean architectural attachment **017188 - Architectural Plans (Final) 02.07.25.pdf** was retrieved through the public portal. A-131 is physical PDF page 10. Its actual title-block issue is **January 31, 2025**; February 7 is part of the attachment filename, not the verified drawing issue date.
- Verified content: cold-formed steel framing takeoff. The workbook Detail sheet contains **457 numeric quantity rows: 449 trade rows and 8 general LS rows**. Summary contains **196 numeric rows: 188 trade rows and 8 general LS rows**. Do not add Detail and Summary together or treat dependent materials derived from repeated lengths/counts as independent measurements. The marked PDF has flattened marks and zero live PDF annotations.
- Status: **retrieved answer-side lead with a material revision gap**. The actual CF-6 takeoff title block is dated **July 30, 2026**, whereas the retrieved clean architectural sheet is issued **January 31, 2025**. Same project identity does not establish that these are interchangeable inputs and answers.
- Seek: the clean drawings and controlling specifications that match the 2026 framing takeoff, addenda/RFIs bridging any changed scope, and native geometry or reproducible high-resolution markup-to-row mapping. Retain the older clean plans as a separately dated input lead until equivalence is demonstrated.

#### Kirksey Office Plaza, Houston / On-Screen Takeoff sample lead

- Official source: [OST 3.98.08.52 installer](https://download.constructconnect.com/Downloads/OST/398/OST3980852.msi), with [ConstructConnect release notes](https://help.constructconnect.com/product-reveal-release-notes-229/on-screen-takeoff-license-key-server-code-licensing-release-notes-2743) and [sample-job support context](https://help.constructconnect.com/takeoff-and-estimating-frequently-asked-questions-244/on-screen-takeoff-or-quick-bid-combining-or-merging-project-bids-jobs-150). Preserve the exact filename **OST3980852.msi**; similarly written filenames in a photograph are not verified URLs.
- Verified content: the official installer was retrieved and its sample content extracted statically without running the installer. The native Walls & Ceilings sample bid has **26 conditions, 1,091 native takeoff objects and 42 page/area-condition total records**, with six linked TIFF sheets: A2.30, A2.31, A2.40, A2.41, A5.32 and A6.30. Condition categories include wall types, drywall ceilings/coves, acoustical ceilings, door frames and corner bead. Conditions, takeoff objects and subtotal records are different populations.
- Status: **retrieved native sample-project lead, still under validation**. These counts establish substantive sample content, not reviewed benchmark coverage. Project title blocks, source geometry, units, calibration, assembly conventions, complete scope and revision alignment still need verification. A separate 5-condition/96-object child bid is a change option replacing X58 with X58MR, not a second independent project.
- Seek: complete project/sheet identity and revision checks, mapping of native objects to condition quantities and source drawings, validated units/calibration, matching specifications and permitted-use terms. Preserve the base bid and change option separately. Do not count this as an admitted package until those checks and the applicable review gates pass.

### Other previously inspected samples

Checked October 10, 2026: the four PDF links below returned HTTP 200 and their contents were inspected. These are **Tier C marketing examples, not gold references**. No complete clean-drawings + specifications + marked-drawings + quantity package was established in this bounded check. Download availability can change; recheck before collection. Reuse, redistribution and training permissions are unknown; the sites display all-rights-reserved notices.

| Example and landing page | Direct downloadable file | Observed evidence | Gaps and unresolved evidence |
|---|---|---|---|
| [Kapolei commercial drywall sample](https://drywalltakeoffservices.us/drywall-estimate-sample/) | [12-page drywall/framing PDF](https://drywalltakeoffservices.us/wp-content/uploads/2026/07/drywall-takeoff-sample-commercial_-Hawai.pdf) | Gypsum board, metal studs and track quantities; color-coded marked floor/locker drawings. Quantity cover and marked sheet A201 identify U-Haul Moving & Storage of Kapolei, Building A, Kapolei, HI 96707: US location evidenced. | Separate clean drawings and specifications not verified. A201 shows December 18, 2024 bid/permit and May 8, 2025 plan-check revisions; takeoff date is blank, so revision alignment remains unverified. Seek the matching issued originals/specifications and confirm quantity basis. |
| Veracity exterior/interior drywall example; discovery URL is the PDF itself (separate landing page not verified) | [6-page drywall PDF](https://veracityestimating.com/wp-content/uploads/2025/02/exterior-and-interior-finishes-drywall-estimate-sample.pdf) | Quantities, costs and marked overlays; project/location redacted. | US project location unknown. Clean drawings, specifications and revision alignment not verified; hold for identity and pairing evidence. |
| [Commercial painting samples](https://paintingtakeoffservices.com/painting-estimate-samples/) | [16-page commercial painting PDF](https://paintingtakeoffservices.com/wp-content/uploads/2025/02/commercial-painting-takeoff-sample.pdf) | Walmart-branded scope, interior/exterior quantities and color-coded architectural/MEP marks. | Location blank/redacted; US location unverified. Brand and units do not establish jurisdiction. Separate clean plans, specifications and revision alignment not verified. |
| [Hotel painting sample landing page](https://paintingtakeoffservices.com/painting-estimate-samples/) | [23-page hotel painting PDF](https://paintingtakeoffservices.com/wp-content/uploads/2025/02/commercial-painting-takeoff-sample-hotel.pdf) | Room/wall/ceiling quantities, room counts and measured architectural drawings. | US project location unverified: an architect's Charlotte, NC address is not a project address. Clean plans, specifications and revision alignment not verified. |

These are already-known leads, not new discoveries. Prioritize missing matching assets for the relevant drywall examples. The two painting-only samples remain secondary historical leads and do not count toward the requested drywall/framing yield. Missing information and unresolved correctness remain explicit limitations; presentation quality alone does not establish reference quality.

