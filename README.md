# Post-Harvest Monitoring Technologies for Artisanal Fisheries

**Research data and evidence extraction for the systematic literature review _Post-Harvest Monitoring Technologies for Artisanal Fisheries: Assessing Suitability under Operational Constraints_.**

## Associated research

**Title:** Post-Harvest Monitoring Technologies for Artisanal Fisheries: Assessing Suitability under Operational Constraints  
**Authors:** Carla de França Pereira; Jair Minoro Abe; Marcus Vinicius Leite; João Glauco Barbosa dos Santos  
**Keywords:** Artisanal fisheries; temperature monitoring; Internet of Things; sociotechnical systems; frugal innovation.

The study investigates whether sensor- and Internet of Things (IoT)-based technologies for monitoring post-harvest fish preservation can operate under the practical constraints of artisanal and small-scale fisheries. Its central argument is that demonstrating technical functionality is not, by itself, sufficient to establish operational suitability on fishing vessels.

In this study, *post-harvest* refers to the handling, stowage, and thermal preservation of fish on board immediately after capture.

## Research questions

**Integrative question:** What limitations, barriers, and gaps remain for the development and adoption of these technologies in the context of artisanal and small-scale fisheries?

- **RQ1 — Performance and Validation Evidence:** How have the technologies been evaluated in the literature, and what evidence exists on their performance under operational conditions relevant to artisanal fisheries?
- **RQ2 — Requirements and Constraints:** Which technical, infrastructural, power, and human requirements constrain the operation of these solutions?
- **RQ3 — Sociotechnical and Frugal Suitability:** To what extent are the characteristics and dependencies of these technologies compatible with the operating conditions of small-scale fisheries, and which barriers remain?

## Review methodology

The systematic literature review follows **Kitchenham and Charters** and the **PRISMA 2020** reporting guidelines. The review scope was structured using **PICOC** (Population, Intervention, Comparison, Outcome, Context), with artisanal and small-scale fishing vessels as the population/context and sensor- or IoT-based post-harvest thermal monitoring as the intervention. Comparisons were recorded when available but were not mandatory for inclusion.

The searches covered **Scopus** (`TITLE-ABS-KEY`) and **Web of Science** (`TS`), supplemented by snowballing. Initial searches were performed in **April 2026**, with updates in May and June and a final update through **2 July 2026**. The strategy combined terms concerning (1) artisanal and small-scale fisheries, (2) IoT and sensors, and (3) monitoring and temperature. The article describes the inclusion and exclusion criteria, screening procedures, and extraction protocol.

### Study selection reported in the manuscript

| PRISMA stage | Records |
| --- | ---: |
| Identified through database searches and snowballing | 467 |
| Duplicates removed | 161 |
| Records screened | 306 |
| Records excluded at screening | 226 |
| Reports assessed for eligibility | 80 |
| Reports excluded because the full text was unavailable | 10 |
| **Studies reported as included in the manuscript** | **70** |

## Research dataset

The extraction matrix is organized in **long format**: one study can have many records, each describing a coded item, its extracted value, and the supporting evidence. The principal identifier is `study_id`; counts of studies must therefore use **distinct study IDs**, not numbers of extraction rows.

The supplied extraction export currently contains **11,677 records for 69 distinct studies**. The manuscript's PRISMA flow reports **70 included studies**. This one-study discrepancy should be reconciled before finalizing public dataset-level statistics. Values derived from the available export should explicitly use **n = 69**, rather than silently substituting the manuscript's total.

The extraction workbook supplied for this project is named `controle_artigos-final.xlsx`. A tab-delimited export of the structured records was also used in the analysis. The exact files published in this repository determine which formats are available for reuse.

### Dataset fields

| Field | Description |
| --- | --- |
| `study_id` | Unique study identifier used to aggregate records belonging to the same publication. |
| `row_order` | Sequence of records within a study. |
| `record_type`, `section_code` | Type of evidence record and its extraction section. |
| `item_code`, `item_name` | Coded item identifier and human-readable description. |
| `value_raw` | Extracted information in its original or recorded wording. |
| `value_normalized` | Standardized representation used for comparative analysis. |
| `classification` | Categorical assessment when defined for the item. |
| `evidence_type` | Provenance category of the evidence or interpretation. |
| `evidence_basis` | Supporting statement or rationale for the entry. |
| `source_page`, `source_section`, `source_object` | Traceability to the publication, including pages, sections, tables, or figures where identified. |
| `rule_applied` | Coding or inference rule used when relevant. |
| `rq`, `picoc` | Links to the research questions and PICOC dimensions. |
| `status`, `reviewer_note` | Review status, uncertainties, conflicts, and analytical notes. |

### Evidence coding

- **R — Reported:** Information explicitly presented in the study.
- **D — Derived:** Information directly derived from reported data using a stated rule.
- **I — Inferred:** Interpretative assessment made during the review, distinct from the authors' claims.
- **NR — Not reported:** Information unavailable or insufficiently documented in the examined source.

Combined labels (such as `R+I`) identify records involving more than one type of evidence. `NR` must **not** be interpreted as a negative technical result. The matrix also distinguishes non-applicable items, ambiguous entries, internal conflicts, and records requiring further review.

### Types of coded records

The dataset includes bibliographic metadata (`META`), thematic scope assessment (`SCOPE`), methodological quality appraisal (`QA`), detailed technical and operational extraction (`EXTRACTION`), sociotechnical/frugal suitability assessment (`STF`), research-question evidence (`RQ`), study synthesis (`SYNTHESIS`), limitations and future work attributed separately to study authors and review authors, cross-study signals (`CORPUS_SIGNAL`), and extraction audit records (`AUDIT`).

A study's `SCOPE_GLOBAL` classification indicates **thematic relevance** (`DIRECT`, `PARTIAL`, `PERIPHERAL`, or `INCONSISTENT`). It must not be used as an automatic exclusion filter when quantifying findings across the full dataset: peripheral studies can contribute relevant evidence on connectivity, energy, maritime operations, or other constraints.

## Analytical framework

The synthesis applies **Sociotechnical Systems (STS)** and **Frugal Innovation (FI)** perspectives through four dimensions:

1. **Infrastructure and energy:** power sources, energy consumption, autonomy, electrical stability, and continuity of operation.
2. **Human, operational, and cognitive factors:** operator intervention, configuration, usability, training needs, and cognitive load.
3. **Connectivity and data architecture:** communication protocols, reliance on external networks, offline data capture, buffering, and resilience to disconnections.
4. **Economic and life-cycle suitability:** acquisition and operating costs, maintenance, repairability, component availability, and economic feasibility.

The matrix also records temperature sensing and metrological validation, preservation outcomes and fish quality indicators, validation environments, and environmental exposure or robustness.

## Principal findings

The review identifies a gap between **technological feasibility** and **demonstrated operational suitability**. Its main findings concern:

- Limited validation of monitoring or preservation systems during sustained, real-world artisanal fishing operations.
- Greater attention to temperature-related measurements than to direct microbiological or sensory evidence of fish quality.
- Incomplete metrological characterization and limited experimental evidence on energy consumption and battery autonomy.
- Insufficient assessment of communication continuity, prolonged disconnections, and recovery behavior.
- Limited verification of resistance to saltwater, humidity, corrosion, vibration, and other maritime conditions.
- Incomplete assessment of human intervention, operational simplicity, cognitive demands, maintenance, repairability, and economic accessibility.

These findings concern the **availability and strength of published evidence**; a lack of reported evaluation does not establish that a technology performs poorly.

## Guidance for reuse

When reproducing descriptive statistics or preparing secondary analyses:

1. Use `study_id` as the unit of analysis and deduplicate before computing article counts.
2. State the denominator for each indicator and identify whether it describes the full available corpus or a justified eligible subset.
3. Distinguish measured performance from specifications, design claims, simulations, and proposed capabilities.
4. Preserve the separation between `R`, `D`, `I`, and `NR`, including source traceability and review notes.
5. Treat the `QA` appraisal and `STF` suitability assessment as different constructs; methodological quality does not, by itself, establish operational compatibility.

This repository provides **literature-derived extraction and analytical records**, not raw telemetry collected from fishing vessels. Findings should be interpreted in the context of the original publications and the review protocol.

## Citation

Until the final publication metadata are available, cite the associated manuscript as:

> Pereira, C. de F., Abe, J. M., Leite, M. V., & dos Santos, J. G. B. (2026). *Post-Harvest Monitoring Technologies for Artisanal Fisheries: Assessing Suitability under Operational Constraints*. Manuscript.

Please cite the original studies when reusing findings extracted from those publications. A publisher DOI or final proceedings reference has not been supplied in the source manuscript and is therefore not listed here.
