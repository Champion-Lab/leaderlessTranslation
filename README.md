# Leaderless Translation Efficiency Analysis

## Overview
Certain bacterial species use regulatory mechanisms to evade the immune system and cause disease. Traditional genome annotation often overlooks leaderless translation, where mRNAs are translated without a 5' UTR or Shine-Dalgarno sequence. This study quantifies leaderless translation efficiency in bacteria using a Python-based computational approach. By analyzing transcription start sites (TSS) and genome reference sequences, we identify ORFs initiating via this mechanism. Across each ORF, translation efficiency is determined by calculating the ratio of ribosomal footprint signal (Translation) to the RNA-seq data (Transcription).

## Features
- Identification of leaderless ORFs based on transcription start sites (TSSs) and a FASTA reference sequence.
- Calculation of translation efficiency by analyzing ribosomal footprint signal relative to RNA-seq data.
- Identification of high-efficiency leaderless transcripts, contributing to the understanding of non-canonical translation mechanisms in bacteria.

## Installation
### Prerequisites
Ensure you have the following dependencies installed:
- Python 3.x
- NumPy
- Pandas
- Biopython
- Matplotlib

### Setup
Clone the repository and navigate to the project directory:
```bash
git clone https://github.com/your-repository/leaderless-translation-analysis.git
cd leaderless-translation-analysis
