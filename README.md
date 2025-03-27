# Leaderless Translation Efficiency Analysis

## Overview
Certain bacterial species use regulatory mechanisms to evade the immune system and cause disease. Traditional genome annotation often overlooks leaderless translation, where mRNAs are translated without a 5' UTR or Shine-Dalgarno sequence. This study quantifies leaderless translation efficiency in bacteria using a Python-based computational approach. By analyzing transcription start sites (TSS) and genome reference sequences, we identify ORFs initiating via this mechanism. Across each ORF, translation efficiency is determined by calculating the ratio of ribosomal footprint signal (Translation) to the RNA-seq data (Transcription).

## Features
- Identification of leaderless ORFs based on transcription start sites (TSSs) and a FASTA reference sequence.
- Calculation of translation efficiency by analyzing ribosomal footprint signal relative to RNA-seq data.
- Identification of high-efficiency leaderless transcripts, contributing to the understanding of non-canonical translation mechanisms in bacteria.

## Installation
### Install Dependencies
Ensure you have the following dependencies installed:
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Biopython
```bash
pip install notebook numpy pandas matplotlib seaborn biopython
```
*To avoid dependency conflicts, it is recommended to create and activate a virtual environment.*

## Setup
Clone the repository:
```bash
git clone https://github.com/your-repository/leaderless-translation-analysis.git
```
### View datasets
The notebook requires the following datasets to run. The `Mtb_inputs` folder within the git repository contains sample data specific to *M. tuberculosis*.
- Genome reference sequence (genome_FASTA, .fasta)
- Table containing coordinate/strand of all known TSSs (TSS, .bed)
- Annotated genes: start base, end base, strand & name (AnnotatedGenes, .bed)
- Ribo-seq data: base values and corresponding ribosomal intensity (Ribosome footprint, .bedgraph)
- RNA-seq data: base values and corresponding RNA intensity (RNA-seq, .bedgraph)
- Ribo-RET data: base values and corresponding ribosomal intensity at initiation site (Ribo-RET footprint, .bedgraph)
- Protein reference sequence (protein_FASTA, .fasta)

### Run the notebook
**Start Jupyter Notebook by running:**
```bash
jupyter notebook
```
Open the `Mtb_leaderless_efficiency.ipynb` Notebook file.<br><br>
**Navigate to the data directory:**<br>
Using the terminal:
```bash
cd leaderless-translation-analysis/Mtb_inputs
```
Using a Jupyter Notebook magic command:
```Python
%cd leaderless-translation-analysis/Mtb_inputs
```
