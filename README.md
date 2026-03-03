
# Metagenome profiling tools

The original motivation was that an increasing number of metagenomic profiling tools are being developed, but it is not always possible to read and evaluate them in detail when they appear. Therefore, I collect them here.

## Acknowledgement

This repository is initialized from a template cloned from the following repository: [genome_assembly_tools](https://github.com/nadegeguiglielmoni/genome_assembly_tools.git)

## Contributing

Adding a software can be done by adding a line in the corresponding CSV file:
* [data/profilers.csv](data/assemblers.csv) for metagenome profiling tools.

Modifications to this readme should be done in the template file of the corresponding section (see [templates](templates)).
Every month, a Github action automatically updates the README using the data and templates, fetching the latest commit date for each software.

## Comment

Metagenomic profiling (classification) tools are rapidly increasing in number and are progressively moving toward finer taxonomic resolutions, such as subspecies and strain levels. This trend makes it increasingly difficult to clearly categorize tools according to the sequencing technologies they support or the taxonomic resolution they truly achieve.

First, some tools were originally developed for NGS data but have later been applied to TGS data. Although updates may have been introduced to accommodate these changes, such modifications are difficult to systematically trace and evaluate.

Second, more and more research focuses on subspecies- and strain-level resolution. Some people attempt subspecies- or strain-level classification using tools that were not originally designed or rigorously evaluated for this purpose. These tools maybe perform profiling because they can assign sequences at a fine-grained taxonomic level, even though their performance at this resolution may be suboptimal.

Therefore, the categorization of tools in here is primarily based on the experimental design and evaluation presented in their original publications. If a tool is reported (e.g. github issues) used at additional taxonomic levels beyond those evaluated in the original study, this is indicated in parentheses.

## Table of contents
* [metagenome profiling tools](#metagenome-profiling-tools)
  * [DNA-to-DNA](#DNA-to-DNA)
  * [DNA-to-protein](#DNA-to-protein)
  * [Marked-based](#Marked-based)




## metagenome profiling tools

### DNA-to-DNA
 
| Profilers | Technology | Profiling_level | Publication | Last update |
|:----------|:---------- |:--------------- |:------------|:------------|
| [Bracken](https://github.com/jenniferlu717/Bracken.git) | NGS | species | [10.7717/peerj-cs.104](https://doi.org/10.7717/peerj-cs.104) | 2025-2 |
| [CAMMiQ](https://github.com/algo-cancer/CAMMiQ.git) | NGS | strain | [10.1038/s41467-022-33869-7](https://doi.org/10.1038/s41467-022-33869-7) | 2021-10 |
| [CLARK](https://github.com/rouni001/CLARK.git) | NGS[;TGS] | species | [10.1186/s12864-015-1419-2](https://doi.org/10.1186/s12864-015-1419-2) | 2024-5 |
| [Centrifuge](https://github.com/DaehwanKimLab/centrifuge.git) | NGS;TGS | species (strain) | [10.1101/gr.210641.116](http://www.genome.org/cgi/doi/10.1101/gr.210641.116) | 2025-6 |
| [Centrifuger](https://github.com/DaehwanKimLab/centrifuge.git) | NGS;TGS | strain | [10.1186/s13059-024-03244-4](https://doi.org/10.1186/s13059-024-03244-4) | 2025-6 |
| [Chimera](https://github.com/LoadStar822/Chimera.git) | NGS | species | [biorxiv](https://www.biorxiv.org/content/10.1101/2025.03.26.645388v1) | 2025-9 |
| [Ganon2](https://github.com/pirovc/ganon.git) | NGS[;TGS] | species (strain) | [10.1093/nargab/lqaf094](https://doi.org/10.1093/nargab/lqaf094) | 2026-2 |
| [KMCP](https://github.com/shenwei356/kmcp.git) | NGS[;TGS] | species (strain) | [10.1093/bioinformatics/btac845](https://doi.org/10.1093/bioinformatics/btac845) | 2023-9 |
| [Kraken2](https://github.com/DerrickWood/kraken2.git) | NGS[;TGS] | species | [10.1186/s13059-019-1891-0](https://doi.org/10.1186/s13059-019-1891-0) | 2026-2 |
| [KrakenUniq](https://github.com/fbreitwieser/krakenuniq.git) | NGS;TGS | species | [10.1186/s13059-018-1568-0](https://doi.org/10.1186/s13059-018-1568-0) | 2023-12 |
| [MADRe](https://github.com/lbcb-sci/MADRe.git) | NGS | strain | [biorxiv](https://www.biorxiv.org/content/10.1101/2025.05.12.653324) | 2025-11 |
| [MegaBLAST](NCBI blast) | NGS;TGS |  | []() | none |
| [MetaCache](https://github.com/muellan/metacache.git) | NGS | species | [10.1093/bioinformatics/btx520](https://doi.org/10.1093/bioinformatics/btx520) | 2025-12 |
| [MetaMaps](https://github.com/DiltheyLab/MetaMaps.git) | TGS | strain | [10.1038/s41467-019-10934-2](https://doi.org/10.1038/s41467-019-10934-2) | 2023-10 |
| [PHLAME](https://github.com/quevan/phlame.git) | NGS | strain (single-species) | [10.1016/j.celrep.2025.116134](https://linkinghub.elsevier.com/retrieve/pii/S2211-1247(25)00905-2) | 2025-8 |
| [PanTax](https://github.com/LuoGroup2023/PanTax.git) | NGS;TGS | strain | [10.1101/gr.280858.125](https://www.genome.org/cgi/doi/10.1101/gr.280858.125) | 2026-3 |
| [Qmatey](https://github.com/bodeolukolu/Qmatey.git) | NGS | strain | [10.1093/bib/bbad351](https://doi.org/10.1093/bib/bbad351) | 2025-10 |
| [StrainEst](https://github.com/compmetagen/strainest.git) | NGS | strain (single-species) | [10.1038/s41467-017-02209-5](https://doi.org/10.1038/s41467-017-02209-5) | 2020-1 |
| [StrainGE](https://github.com/broadinstitute/StrainGE.git) | NGS | strain (single-species) | [10.1186/s13059-022-02630-0](https://doi.org/10.1186/s13059-022-02630-0) | 2024-10 |
| [StrainR2](https://github.com/BisanzLab/StrainR2.git) | NGS | strain (single-species) | [10.1093/bioinformatics/btaf440](https://doi.org/10.1093/bioinformatics/btaf440) | 2026-2 |
| [StrainScan](https://github.com/liaoherui/StrainScan.git) | NGS | strain (single-species) | [10.1186/s40168-023-01615-w](https://doi.org/10.1186/s40168-023-01615-w) | 2024-4 |
| [Sylph](https://github.com/bluenote-1577/sylph.git) | NGS; TGS | species | [10.1038/s41587-024-02412-y](https://doi.org/10.1038/s41587-024-02412-y) | 2026-2 |
| [Taxor](https://github.com/JensUweUlrich/Taxor.git) | TGS | species | [10.1101/gr.278623.123](https://www.genome.org/cgi/doi/10.1101/gr.278623.123) | 2025-8 |
| [UniqSketch](https://github.com/amazon-science/uniqsketch.git) | NGS | strain | []() | 2024-9 |

### DNA-to-protein
 
| Profilers | Technology | Profiling_level | Publication | Last update |
|:----------|:---------- |:--------------- |:------------|:------------|
| [Kaiju](https://github.com/bioinformatics-centre/kaiju.git) | NGS[;TGS] | species | [10.1038/ncomms11257](https://doi.org/10.1038/ncomms11257) | 2025-1 |
| [MEGAN-LR](https://uni-tuebingen.de/fakultaeten/mathematisch-naturwissenschaftliche-fakultaet/fachbereiche/informatik/lehrstuehle/algorithms-in-bioinformatics/software/megan6) | TGS | strain | [10.1186/s13062-018-0208-7](https://doi.org/10.1186/s13062-018-0208-7) | 2018 |
| [MMseqs2](https://github.com/soedinglab/MMseqs2.git) | NGS[;TGS] | forma;varietas;subspecies;species | [10.1093/bioinformatics/btab184](https://doi.org/10.1093/bioinformatics/btab184) | 2026-2 |

### Markers
 
| Profilers | Technology | Profiling_level | Publication | Last update |
|:----------|:---------- |:--------------- |:------------|:------------|
| [Melon](https://github.com/xinehc/melon.git) | TGS | species | [10.1186/s13059-024-03363-y](https://doi.org/10.1186/s13059-024-03363-y) | 2025-4 |
| [MetaPhlAn4](https://github.com/biobakery/MetaPhlAn.git) | NGS;TGS(v4.2.2) | species | [10.1038/s41587-023-01688-w](https://doi.org/10.1038/s41587-023-01688-w) | 2025-12 |
