# Getting Started

## 1.0: Overview
The **G**enome **A**ssembly **E**valuation **M**etrics and **R**eporting (GAEMR) package is an assembly analysis framework composed a number of integrated modules. These modules can be executed as a single program to generate a complete analysis report, or executed individually to generate specific charts and tables. GAEMR standardizes input by converting a variety of read types to Binary Alignment Map (BAM) format, allowing a single input format to be entered into GAEMR’s analysis pipeline, hence enabling the generation of standard reports.

GAEMR’s analysis philosophy is centered on contiguity, correctness, and completeness -- how many pieces in an assembly composed of, how well those pieces accurately represent the genome sequenced, and how much of that genome is represented by those pieces. By performing over twenty different analyses based on these principles, GAEMR gives a clear picture of the condition of a genome assembly. For a broadly-defined list of these analyses, see the Features section below.

## 1.1: Features
The features of GAEMR are as follows:

* Modular design that allows all analyses to be created with a single command but is flexible enough to allow users to request specific reports
* Assembly statistics and details
* Read alignment statistics
* Kmer analysis
* Gap end reports
* Reference analysis
* Blast reports
* rRNA details
* HTML and text reporting formats

## 1.2: System Requirements & Dependencies
GAEMR and its modules are written in the Python programming language and run in a UNIX environment. The third-party packages below are required by GAEMR. Please contact your systems administrator to see if you have them installed.

**Programming Language**: Python 2.7 with Biopython, Matplotlib, Optparse, NumPy and Pysam modules

**Alignment Software**: BWA, Bowtie 2, Blast+ and Nucmer

**SAM/BAM** Utilities: Picard, SAMtools

**Classification**: RNAmmer, RDP-classifier 2.4, NCBI taxonomy dump

## 1.3: Installation
Follow the steps below to set up GAEMR:

1. Download the GAEMR package from the download site.
2. Move or copy the package to the Unix directory where you’d like GAEMR to be installed.
3. Inside this directory, unpack the the file by typing “tar -xzvf GAEMR-1.0.0.tar.gz”. A directory called GAEMR-1.0.0 will be created.
4. Read and follow the instructions in the README.txt file located  inside the GAEMR-1.0.0 directory.

## 1.4: Next Steps
The GAEMR website is designed to be user-friendly and informative.  Throughout the website, you will find words with tool-tip definitions to help users unfamiliar with bioinformatics and genomics jargon. Each page is composed of sections that can be expanded or collapsed to help users focus only on the sections of interest.

The website is divided into the following pages to make accessing and learning how to use GAEMR as easy as possible:

### 1.0: Getting Started

This page, where you will find an overview of GAEMR, as well as features, system requirements, dependencies, and installation instructions.

### 2.0 User’s Guide

The User’s Guide is designed with a ‘how-to’ approach ideal for those just getting started with GAEMR. The guide contains basic usage instructions and tutorials on how to create and understand GAEMR output.

### 3.0 Reference Manual

The reference manual is intended for those familiar with GAEMR who want to access the full complement of GAEMR arguments or understand and execute individual GAEMR modules.  Examples of all tables and charts produced by GAEMR can also be found here.

### 4.0 Downloads

The downloads section contains available versions of the GAEMR package as well as sample data used in the the User’s Guide tutorials.

## 1.5: Support
GAEMR is supported through the GAEMR-help mailing list. Changes are reported on the Change Log. Both may be accessed from the GAEMR homepage.
