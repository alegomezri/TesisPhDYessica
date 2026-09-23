# Connectivity-Based Deep Learning for EEG Decoding in Brain-Computer Interfaces

LaTeX source repository for the doctoral thesis of **Yessica Alejandra Gómez Rivera**.

**Doctoral program:** Ph.D. in Engineering - Automation  
**Institution:** Universidad Nacional de Colombia, Manizales Campus  
**Director:** Prof. Dr. Andrés Marino Álvarez-Meza  
**Co-director:** Prof. Dr. David Cárdenas-Peña

## Repository organization

| Location | Contents |
| --- | --- |
| `main_yessica.tex` | Root LaTeX document used to compile the complete thesis. |
| `Front_Matter/` | Acknowledgements, abstract, abbreviations, and acronym definitions. |
| `Chapters/Chapter_01_Preliminaries/` | Motivation, problem statement, and state of the art. |
| `Chapters/Chapter_02_Aims/` | General and specific research objectives. |
| `Chapters/Chapter_03_Outline_and_Contributions/` | Thesis organization, evaluated datasets, and contributions. |
| `Chapters/Chapter_04_EEG_GCIRNet/` | Gaussian connectivity-driven EEG imaging contribution. |
| `Chapters/Chapter_05_TEKTE_Net/` | Takens-based kernel Transfer Entropy contribution. |
| `Chapters/Chapter_06_CTE_Net/` | Transformer-based directed Transfer Entropy contribution for ADHD classification. |
| `Chapters/Chapter_07_Final_Remarks/` | Conclusions, future work, and academic products. |
| `Appendices/` | Supplementary thesis material. |
| `Figures/` | Figures, diagrams, and data files used to generate plots. |
| `References.bib` | Complete bibliography database. |
| `dtvstyle.bst` | Bibliography style required by the document. |

## Compile on Overleaf

1. Download this repository as a ZIP file.
2. In Overleaf, select **New Project > Upload Project** and upload the ZIP file.
3. Open **Menu** and set `main_yessica.tex` as the **Main document**.
4. Select **pdfLaTeX** as the compiler and recompile.

## Compile locally

A complete TeX Live installation is recommended. From the repository root, run:

```bash
latexmk -pdf -interaction=nonstopmode -file-line-error main_yessica.tex
```

To remove auxiliary compilation files:

```bash
latexmk -c
```

## Compiled thesis PDF

The compiled thesis PDF is intentionally not tracked in the repository. Final compiled versions should be published as assets under **GitHub Releases**, while the repository retains the reproducible LaTeX source.

## Automatic GitHub build

The workflow in `.github/workflows/compile-thesis.yml` compiles `main_yessica.tex` after every push or pull request. The resulting PDF can be downloaded from the corresponding run in the **Actions** tab as the `thesis-pdf` artifact.

## Related implementations

- [EEG-GCIRNet](https://github.com/alegomezri/EEG-GCIRNet)
- [TEKTE-Net](https://github.com/alegomezri/TEKTE-Net)
- [EEG-TACT](https://github.com/alegomezri/EEG-TACT)
- [CTE-Net](https://github.com/alegomezri/CTE-Net)

## Notes

- This repository contains the complete thesis manuscript and all files required to reproduce the document.
- Implementation code remains in the related repositories listed above.
- The LaTeX source is the authoritative version of the manuscript.
