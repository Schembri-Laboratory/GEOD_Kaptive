<a href="[https://github.com/klebgenomics/Kaptive/](https://github.com/klebgenomics/Kaptive/)">
    <img align="right" src="https://github.com/klebgenomics/Kaptive/blob/master/docs/assets/logo.png?raw=true" alt="Kaptive" width="200">
</a>

# The Genomic _Escherichia coli_ O-antigen Database (GEOD)
A database for accurate and comprehensive O-typing of _E. coli_ using [Kaptive](https://github.com/klebgenomics/Kaptive/).


## How to use 👉
Run the following command to install the database

```bash
kaptive db add EC_Oag Schembri-Laboratory GEOD_Kaptive
```
Example Usage
```bash
kaptive assembly ecol_o assemblies/*.fasta.gz > serotypes.tsv
```
## Typing and Nomenclature 📝
### Cannonical O-antigens ✅
All cannonical O-types (O1-O187) match perfectly to their  O-locus (OL). This also holds true for subtypes. For example, O1 maps to OL1, O25b maps to OL25b.
### Putative O-antigens ❓
For putatative O-antigens given a name by others, the original O-type designation has been retained. However, they have been mapped to OL types from OL188-OL216.

The putative O-antigen loci found by Morris et al. (2026) have been assigned OL types OL217-OL264. Three of these (OL226, OL230 and OL251) have been assigned a corresponding O-type as they have previously been phenotypically confirmed.

For a complete list see table S4 in the following publication.
### High-Similarity Groups
35 O-antigens belong to high-similarity groups (Gp1-16), where members of the group share >95% nucleotide identity [2].
All but Gp11 are annotated in GEOD. Kaptive cannot reliably differentiate O-antigens in the same group, hence caution is advised in interpreting results for these O-types.

|     Group    |     O-antigens                  |
|--------------|---------------------------------|
|     Gp1      |     O20, O137                   |
|     Gp2      |     O28ac, O42                  |
|     Gp3      |     O118, 151                   |
|     Gp4      |     O90, O127                   |
|     Gp5      |     O123, O186                  |
|     Gp6      |     O46, O134                   |
|     Gp7      |     O2, O50                     |
|     Gp8      |     O107, O117                  |
|     Gp9      |     O17, O44, O73, O77, O106    |
|     Gp10     |     O13, O129, O135             |
|     Gp12     |     O18ab, O18ac                |
|     Gp13     |     O124, O164                  |
|     Gp14     |     O62, O68                    |
|     Gp15     |     O89, O101, O162             |
|     Gp16     |     O169, O183                  |


### Phenotype Logic 🧠

| Phenotype      | Inactive Genes        |
|----------------|-----------------------|
| Rough LPS      | _wzx, wzm, wzt, wbbL_ |
| Semi-Rough LPS | _wzy_                 |

More phenotype logic will be added in future updates.




## References 📚
[^1]: Stanton TD, Hetland MAK, Löhr IH, Holt KE, Wyres KL. Fast and
    Accurate in silico Antigen Typing with Kaptive 3.
    2025 _Microbial Genomics_ 11(6):001428.
    <https://doi.org/10.1099/mgen.0.001428>

[^2]: Iguchi A, Iyoda S, Kikuchi T, et al. A complete view of the genetic diversity of the Escherichia coli O-antigen biosynthesis gene cluster. DNA Res. 2015;22(1):101-107. <doi:10.1093/dnares/dsu043>
