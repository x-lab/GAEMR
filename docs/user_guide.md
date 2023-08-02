# User’s Guide

## 2.0: Basic Usage
### 2.0.1: FILE PREPARATION
Before running GAEMR, please ensure that the input files are formatted correctly as indicated here:

[Reference Manual -- Section 3.0: Input Format Requirements]()

### 2.0.2: BASIC COMMANDS
GAEMR’s modular design affords users the flexibility to run basic commands for users with a limited data set (such as a single FASTA file), users with a full data set (AGP, BAM, and FASTA files), and anything in between. Only the basic usage is outlined in this section. Those interested in more advanced instructions may read Section 2.1: Tutorials.

To see the all the command line arguments from the terminal prompt, call GAEMR with either of the help arguments (-h, --help):

```sh
GAEMR.py --help
```

These options are also described here:

[Reference Manual -- Section 3.1: GAEMR Arguments]()

GAEMR requires a minimum of a scaffolds or contigs FASTA file in order to run, as most arguments will use default values if none are provided by the user (see Section 3.1, linked above, for default values). To run GAEMR at its most basic level, either a contigs FASTA file or a scaffolds FASTA file is required. Either of these files may be indicated with either the short form argument (-c or -s) or the long form argument(--contigs or --scaffolds) as follows:


```sh
GAEMR.py -c contigs.fasta
```

or
```sh
GAEMR.py -scaffolds=scaffolds.fasta
```

Running GAEMR with only a scaffolds FASTA will generate the following tables and charts described in the Reference Manual:


| Analysis Section | Tables and Charts Produced |
| ---------------- | -------------------------- |
| Assembly Stats   | Basic Assembly Stats, Cumulative Sizes |
| Kmer Analysis    | Kmer Copy Number |
| Gap End Analysis | Gap End Analysis Table, CG Sizes, CG Distinctness, CG Copy Number, CG GC, UE Distinctness, UE Copy Number, UE GC |
| Blast Analysis   | Blast Taxonomy Details, Blast Bubbles, Blast Heat Map |
| Assembly Details | Contig Details, Scaffold Details |

Users with a de novo assembly FASTA file, BAMs, and AGP files can produce a larger set of charts and tables by running GAEMR as follows:

```sh
GAEMR.py --scaffolds=scaffolds.fasta --read_list=reads.csv --agp=assembly.agp
```

To add reference-alignment-based data for an assembly, specify a reference with the --reference(-r) option:
```sh
GAEMR.py --scaffolds=scaffolds.fasta --read_list=reads.csv --agp=assembly.agp --reference=reference.fasta
```
