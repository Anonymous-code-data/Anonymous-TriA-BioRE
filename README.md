# Exploring Pair-Aware Triangular Attention for Biomedical Relation Extraction

This repository contains the code and data for the paper "Exploring Pair-Aware Triangular Attention for Biomedical Relation Extraction".

## TriA-BioRE

We propose a novel Triangular Attention framework for Biomedical Relation Extraction (called TriA-BioRE) to comprehensively capture pair-aware representations in the biomedical domain. Specifically, we present a triangular attention module, including two triangular multiplications utilizing outgoing and incoming edges, and two triangular self-attention operations centered on the starting and ending nodes, respectively, together to enhance the pair-level modeling omnidirectionally for better BioRE performance.

## Requirements

```
python>=3.6
pytorch==1.10.2
transformers==4.18.0
numpy==1.19.5
```

## Quick Start

Put the `CDR` dataset (including `train_filter.data`, `dev_filter.data` and `test_filter.data`) into folder `./dataset/cdr`.

Put the `GDA` dataset (including `train.data`, `dev.data` and `test.data`) into folder `./dataset/gda`.

Put the `BioRED` dataset (including `train_filter.data`, `dev_filter.data` and `test_filter.data`) into folder `./dataset/biored`.

### Train `TriA-BioRE`

```
python train_triangle.py
```