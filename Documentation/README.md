# Data Dictionary

## Dataset

- **File:** `Data/Cybersecurity_Ontology_Corpus.xlsx`
- **Worksheet:** `Ontology Corpus`
- **Unit of observation:** one cybersecurity ontology record per row
- **Number of records:** 231, excluding the header row

## Fields

| Column | Field | Data type | Required | Description | Example / permitted values |
|---:|---|---|:---:|---|---|
| A | `ID` | Text identifier | Yes | Stable ontology identifier assigned within the corpus. Values must be unique and should not be renumbered when the dataset is updated. | `Onto-1`, `Onto-231` |
| B | `Source` | Text / hyperlink | Yes | BibTeX citation key of the publication that introduced or described the ontology. In the Excel file, the citation key is hyperlinked to the original publication or its persistent landing page. | `syed_uco_2016` |
| C | `Focus` | Text | Yes | Concise description of the ontology’s stated focus or purpose, reproduced from the ontology corpus. | `Unified Cybersecurity Ontology` |
| D | `ECJRC_Primary_Domain` | Categorical text | Yes | Code for the ontology’s primary domain under the EC JRC Cybersecurity Taxonomy. This records the main domain only; the ontology may cover additional domains. | `SMG`, `OIHDF`, `SHSE` |
| E | `Semantic_Availability` | Categorical text | Yes | Indicates whether a publicly accessible, machine-readable semantic representation was located and inspected. | `Yes`, `No` |
| F | `Semantic_Resource_URL` | Hyperlink or blank | Conditional | For semantically available ontologies, the cell displays the ontology name or acronym and links to the semantic resource or repository. The cell is blank when no public semantic resource URL was recorded. | Display text: `UCO`; target: ontology URL |
| G | `Source_SLR` | Text / hyperlink | Yes | BibTeX citation key of the systematic literature review through which the ontology source was identified. The value is copied from the curated corpus and refers to one of the nine selected reviews. In the Excel file, it is hyperlinked to the review publication. | `hasan_systematic_2025` |

## EC JRC Primary-Domain Codes Used in the Dataset

| Code | Domain |
|---|---|
| `AAAC` | Assurance, Audit, Assessment and Certification |
| `EAT` | Education and Training |
| `HA` | Human Aspects |
| `IAM` | Identity and Access Management |
| `LA` | Legal Aspects |
| `NDS` | Network and Distributed Systems |
| `OIHDF` | Operational Incident Handling and Digital Forensics |
| `SHSE` | Software and Hardware Security Engineering |
| `SM` | Security Measurements |
| `SMG` | Security Management and Governance |
| `TF` | Theoretical Foundations |
| `TMAA` | Trust Management, Assurance, and Accountability |

The full EC JRC taxonomy contains additional domains. The table above lists only the primary-domain codes present in this dataset.

