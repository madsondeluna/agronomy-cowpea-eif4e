# Unveiling Three Functionally Diverse Isoforms of eIF4E in Cowpea Through a Multi-Omics Approach

Repository for the datasets, structural models, analysis outputs, and computational workflows associated with the manuscript:

```markdown
Luna-Aragão, M. A. de, Andrade, F. A. de, Penna, S. R. M., Maciel, L. S., Rodrigues-Paixão, L. M., Lemos, A. B., Ferreira, J. D. C., Aragão, F. J. L., Pandolfi, V., & Benko-Iseppon, A. M. (2025). Unveiling Three Functionally Diverse Isoforms of eIF4E in Cowpea Through a Multi-Omics Approach. Agronomy, 15, xxx. https://doi.org/10.3390/xxxxx
```

## Manuscript status

This repository supports a manuscript currently in **pre-proof / production stage**.  
Minor changes may still occur in the final published version, including:

- article metadata
- volume, issue, and page numbers
- DOI
- supplementary file numbering
- figure numbering
- wording in methods/results sections

Until the final version is released, please treat this repository as the **author-curated public data companion** for the study.

## Overview

The eukaryotic translation initiation factor 4E (eIF4E) family plays a central role in cap-dependent translation and is also recurrently associated with susceptibility or resistance to potyviruses in plants. In cowpea (*Vigna unguiculata*), this repository documents a multi-omics and structural bioinformatics investigation of three cap-binding protein isoforms:

- **eIF4E**
- **eIF(iso)4E**
- **nCBP**

The study integrates sequence mining, chromosomal mapping, gene structure inspection, synteny analysis, phylogenetic reconstruction, structural modeling, model validation, molecular dynamics simulations, and electrostatic surface analysis to characterize these isoforms at genomic, evolutionary, and structural levels.

## Why this repository exists

This repository was created to:

- make the study reproducible
- provide public access to curated sequence and structural datasets
- expose the computational logic behind the analyses
- preserve raw and processed outputs used in the manuscript
- facilitate downstream reuse for allele mining, comparative genomics, structural biology, and crop improvement studies

## Study rationale

Cowpea is an agronomically important legume and a major crop in several regions of the world. Members of the eIF4E family are biologically relevant because they simultaneously:

- regulate cap-dependent protein synthesis
- participate in RNA metabolism
- may act as host susceptibility factors exploited by potyviruses such as CABMV

Despite the relevance of these proteins, the structural determinants and evolutionary organization of the cowpea eIF4E family were still insufficiently characterized. This repository addresses that gap by providing data and analyses for the three identified cowpea isoforms.

## Main findings

The study supports the following main conclusions:

1. **Three paralogous eIF4E-family genes were identified in cowpea**, corresponding to **nCBP**, **eIF4E**, and **eIF(iso)4E**.
2. These genes are located on **chromosomes 4, 6, and 7**, respectively.
3. The family shows **high synteny with *Phaseolus vulgaris*** and a genomic organization compatible with **dispersed duplication events**.
4. Phylogenetic analyses support the evolutionary separation of **nCBP** from the canonical **eIF4E / eIF(iso)4E** lineages.
5. All modeled proteins preserve the **canonical “cupped hand” fold** characteristic of eIF4E-family cap-binding proteins.
6. Molecular dynamics analyses indicate overall structural stability for all isoforms across simulated systems.
7. **eIF(iso)4E** showed the strongest signature of **compactness and structural stability**, making it a particularly relevant target for future functional and applied studies.
8. Electrostatic surface analyses revealed a **conserved electropositive cap-binding cleft**, consistent with functional competence for mRNA cap recognition.

## Experimental and computational scope

The repository covers data and outputs related to the following analytical layers.

### 1. Sequence mining and isoform identification

Annotated genes encoding eIF4E-family proteins were retrieved from public plant genome resources and validated by similarity searches against experimentally characterized sequences. This step supported the identification of cowpea orthologs/paralogs for:

- eIF4E
- eIF(iso)4E
- nCBP

### 2. Primer design and experimental sequence acquisition

Isoform-specific primers were designed to amplify the complete coding sequences of the three genes from cDNA derived from six cowpea cultivars with contrasting CABMV phenotypes.

The cultivars analyzed were:

- Bajão
- Boca Negra
- BR14 Mulato
- IT85F-2687
- Pingo de Ouro
- Santo Inácio

These experimental sequences provide the cultivar-level foundation for the comparative analyses presented here.

### 3. Chromosomal mapping and structural genomics

Transcript/gene sequences were mapped to the reference cowpea genome to establish:

- chromosomal location
- exon-intron organization
- structural conservation among isoforms
- gene family expansion patterns

### 4. Synteny and comparative genomics

Comparative analyses were used to examine collinearity and genomic conservation between cowpea and other legumes, especially:

- *Phaseolus vulgaris*
- *Glycine max*
- *Lens culinaris*

These analyses help contextualize the origin, conservation, and rearrangement patterns of the eIF4E gene family in legumes.

### 5. Phylogenetic reconstruction

A curated multi-species dataset was used to reconstruct the evolutionary history of the eIF4E family in Fabaceae and related taxa. Trees were inferred using both:

- **Maximum Likelihood**
- **Neighbor-Joining**

This enabled the discrimination of major isoform classes and the positioning of cowpea proteins within a broader evolutionary framework.

### 6. Protein sequence comparison and conserved signatures

Translated amino acid sequences were aligned to identify:

- conserved motifs
- hallmark aromatic residues
- domain preservation
- variable regions, especially in N-terminal segments

This step supports the interpretation of how sequence conservation relates to structural and functional maintenance.

### 7. Structural modeling and validation

Three-dimensional models were generated for all isoforms and assessed using multiple quality metrics. Validation procedures were included to evaluate:

- confidence of predicted folds
- stereochemical plausibility
- energetic reasonableness
- suitability for downstream simulation

### 8. Molecular dynamics simulations

Molecular dynamics simulations were performed to move beyond static structural predictions and assess the conformational behavior of the proteins over time. The analyses include:

- **RMSD**
- **RMSF**
- **B-factor mapping**
- **Radius of Gyration (RG)**
- **Hydrogen Bonds (HBs)**
- **Solvent Accessible Surface Area (SASA)**
- **Minimum Distance Matrices (MDMAT)**

These outputs are relevant for evaluating stability, flexibility, compactness, and preservation of tertiary contacts.

### 9. Electrostatic surface potential

Electrostatic calculations were used to characterize the physicochemical landscape of the cap-binding region. The conserved electropositive cleft observed across models supports the structural interpretation of ligand recognition.

## Repository contents

This repository is organized to separate raw data, processed outputs, structural files, and executable workflows.

```text
.
├── README.md
├── LICENSE
├── CITATION.cff
├── .gitignore
├── data/
│   ├── raw/
│   │   ├── sanger_traces/
│   │   ├── reference_sequences/
│   │   ├── genome_annotations/
│   │   └── primers/
│   ├── processed/
│   │   ├── cds/
│   │   ├── amino_acid_sequences/
│   │   ├── curated_phylogeny_dataset/
│   │   ├── alignments/
│   │   ├── chromosomal_coordinates/
│   │   └── synteny_tables/
│   └── metadata/
│       ├── sample_metadata.tsv
│       ├── cultivar_phenotypes.tsv
│       └── file_manifest.tsv
├── results/
│   ├── sequence_identity/
│   ├── gene_structure/
│   ├── chromosomal_mapping/
│   ├── synteny/
│   ├── phylogeny/
│   ├── domain_annotation/
│   ├── structural_validation/
│   ├── md/
│   │   ├── rmsd/
│   │   ├── rmsf/
│   │   ├── bfactor/
│   │   ├── rg/
│   │   ├── hbonds/
│   │   ├── sasa/
│   │   └── mdmat/
│   └── electrostatics/
├── models/
│   ├── alphafold3/
│   │   ├── pdb/
│   │   ├── pae/
│   │   ├── plddt/
│   │   └── validation_reports/
│   └── superpositions/
├── figures/
│   ├── main/
│   └── supplementary/
├── scripts/
│   ├── sequence_processing/
│   ├── phylogeny/
│   ├── synteny/
│   ├── structure/
│   ├── md/
│   └── electrostatics/
└── docs/
    ├── methods/
    ├── software_versions/
    └── workflow_notes/
