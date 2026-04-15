# Convergent Evolution of Iron Acquisition Pathways in Cefiderocol-Resistant   *Pseudomonas aeruginosa*: Defining the Dark Matter Resistome

## Overview

This repository contains all data, figures, results, and scripts for the systematic review and bioinformatic analysis titled:

**"From Dark Matter to Diagnostics: A Systematic Review and Bioinformatic Analysis of Non-Canonical Iron-Uptake Genes Driving Cefiderocol Resistance in *Pseudomonas aeruginosa*"**

The study identifies and characterises **36 non-canonical "dark matter" genes** (iron‑uptake genes absent from canonical AMR databases) that are consistently mutated in cefiderocol‑resistant *P. aeruginosa*. Key findings include functional enrichment in iron homeostasis, clone‑specific mutation signatures, drug target prioritisation, and the design of a validated multiplex PCR primer panel.

---

## Repository Structure
AMR_Dark_Matter_Study/
├── data/ # All CSV data files
├── figures/ # Publication‑ready PDF figures
├── results/ # Bibliometric and summary tables
├── scripts/ # All Python analysis scripts
└── README.md # This file

---

## Data (`data/`)

| File | Description |
|------|-------------|
| `included_14_papers.csv` / `included_22_papers.csv` | Final included studies |
| `top_50_papers.csv` | EmbedSLR semantic ranking output |
| `dark_matter_genes.csv` | List of 36 consolidated dark matter genes |
| `clone_mutation_data.csv` | Clone‑specific mutation signatures |
| `drug_target_priority_results.csv` | Multi‑parameter drug target prioritisation |
| `final_primer_results_VALIDATED.csv` | Validated primer designs |
| `final_primer_results_TOP10.csv` | Top 10 primer candidates |
| `insilico_pcr_results.csv` | *In silico* PCR validation results |
| `bibliometric_summary.csv` | Bibliometric metrics for final corpus |

---

## Figures (`figures/`)

| File | Description |
|------|-------------|
| `prisma_flow.pdf` | PRISMA flow diagram of study selection |
| `enrichment_final.pdf` | Functional enrichment bar chart (STRING) |
| `clone_combined_panel.pdf` | Heatmap + stacked bar chart of clone‑specific mutations |
| `clone_heatmap.pdf` | Mutation distribution heatmap |
| `clone_mutation_barchart.pdf` | Stacked bar chart with MIC annotations |
| `clone_mutations_panel.pdf` | Multi‑panel clone signature visualisation |
| `dark_matter_gene_frequencies_horizontal.pdf` | Frequency distribution of 36 genes |
| `panel_plot_with_legend.pdf` | Combined panel: author network, gene network, publication trend |
| `author_collaboration.pdf` | VOSviewer author collaboration network |

---

## Results (`results/`)

| File | Description |
|------|-------------|
| `bibliometric_summary.csv` | Document counts, authors, sources, co‑authorship metrics |
| `dark_matter_summary.csv` | Consolidated frequency of each dark matter gene |

---

## Scripts (`scripts/`)

| Script | Purpose |
|--------|---------|
| `01_embedslr_ranking.py` | Semantic ranking using EmbedSLR |
| `02_identify_dark_matter.py` | Keyword‑based identification of dark matter papers |
| `03_clone_analysis.py` | Clone‑specific mutation heatmap and bar charts |
| `03_create_prisma.py` | PRISMA flow diagram generation |
| `03_screening_template.py` | Creation of screening template with 6 inclusion criteria |
| `04_create_figure.py` | General figure generation (gene frequencies, etc.) |
| `04_enrichment_analysis.py` | STRING API enrichment analysis and plotting |
| `05_export_ris.py` | RIS export for VOSviewer bibliometric mapping |
| `05_prisma_flow.py` | Alternative PRISMA flow script |
| `restart_session.py` | Utility to mount Drive and reload data |

All scripts are compatible with **Python 3.12** and require: `pandas`, `matplotlib`, `numpy`, `networkx`, `requests`, `openpyxl`.

---

## Key Findings

- **36 dark matter genes** identified (e.g., *piuC*, *fptA*, *pirR*, *piuA*, *tonB*, *cirA*)
- **Functional enrichment** in iron homeostasis, siderophore transport, and TonB‑dependent receptor activity (FDR < 0.05)
- **Clone‑specific signatures**: ST175 (8 mutations, up to 64× MIC), ST235 (3 mutations, 2–5×), ST111 (*cpxS*/*pbp3*), ST266 (*fptA* G273R), ST312 (*piuCD*–*ampD* deletion)
- **Drug target prioritisation** and **multiplex PCR primer panel** for rapid detection

---

## Methodology

The study followed **PRISMA guidelines** and used **EmbedSLR** (all‑distilroberta‑v1) for semantic ranking. Full details are available in the manuscript.

---

## Citation

If you use this repository, please cite the associated manuscript (available upon publication).

---

## License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.

---

## Contact

For questions or requests, please contact the corresponding author.
