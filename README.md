# Neural Organoid Mechanotransduction

Bioinformatics internship project with Prof. Akansha Jain, exploring ECM biology and mechanotransduction in human neural organoids using the [Zhisong He neural organoid atlas](https://github.com/theislab/neural_organoid_atlas).

## Research Questions

- **Integrin profiling**: Do different cell types (e.g., telencephalic progenitors) have distinct integrin profiles that determine which ECM components they can respond to?
- **ECM remodeling dynamics**: When are MMPs and TIMPs produced, and which time periods show the most active tissue reshaping?
- **ECM production**: Which cells produce the most ECM, when, and what structural components?
- **ECM sensing**: Which cells are sensing the ECM, and what is their mechanosensing competence?
- **Mechanotransduction pathways**: How are Hippo/YAP and other mechanosensing pathways engaged across protocols and timepoints? Do they influence cell fate?
- **Understudied ECM genes**: Do matricellular proteins or other rarely studied ECM genes show interesting expression in neural organoids?
- **ECM & protocol comparison**: Are mechanotransduction genes differentially expressed in Matrigel vs. non-Matrigel protocols?
- **Cell–cell communication**: Is there endogenous ECM-based signaling between cell populations?
- **Regional identity & ECM**: How do regional identities correlate with ECM signatures?
- **Morphogens & mechanosensing**: In guided protocols, how do morphogens influence mechanosensing?
- **ECM & migration**: Does ECM influence cell migration?
- **Gene regulatory networks**: Which transcription factors drive ECM gene expression in specific cell types?

## Approach

Single-cell transcriptomic analysis using Scanpy, including:
- Pathway scoring (`sc.tl.score_genes()`) for YAP activity, integrin expression, ECM production, and mechanosensing competence
- Differential expression between Matrigel vs. non-Matrigel conditions
- Correlation of pathway scores across cell types and developmental time
- GRN inference to identify transcription factors regulating ECM genes

## Data

The atlas data (`hnoca_cleanedmeta.h5ad`, ~18.7 GB) is not tracked in this repo due to size. See the [neural organoid atlas](https://github.com/theislab/neural_organoid_atlas) for data access.

## Structure

```
├── Findings.pptx                       # Presentation of findings
├── Mechanotransduction/
│   ├── data/                           # Local data (gitignored)
│   └── notebooks/
│       ├── 01_curate_atlas_nick.ipynb
│       ├── 02_nick_preprocessing_and_integration.ipynb
│       ├── smaller_atlas_ECM.ipynb
│       └── Zhisong/                    # Reference notebooks from Zhisong He
```
