
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
  * [DNA-to-DNA](DNA-to-DNA)
  * [DNA-to-protein](DNA-to-protein)
  * [Marked-based](Marked-based)



