---
layout: single
title: "CMap LINCS Workshop 2020 Summary"
categories:
  - Blog
mathjax: true
---
별 내용 없음.

## Why not use GSE92742/GSE70138?
Q: What is the difference between data from GEO, LINCS portal (lincsproject.org, lincs-dcic.org), and CLUE?

A: The Connectivity Map analysis platform (clue.io) contains L1000 data and other perturbagen datasets made from a variety of public, philanthropic, and industrially funded projects. NIH-supported LINCS data is deposited into GEO twice per year.  That same data from GEO is also imported by the LINCS DCIC into the LINCS portal at lincsproject.org, so that it is inter-operable with other LINCS data. So, data in CLUE is a **superset** of public domain L1000 datasets.

# Day 1, Data Access

## Introduction
- LINCS: **L**ibrary of **I**ntegrated **N**etwork-Based **C**ellular **S**ignatures  
- Motivation: mRNA based signatures of cell state to link diseases, drugs, and genes
- Perturbagen > Cell > mRNA expression
- L1000 assay for scalability: experimentally measure 1,000 genes, infer 11350 genes
- 2017, 1.3M profiles, 28,000 perturbagens, 80 cell lines.
- 2020, 3M profiles, 81,979 perturbagens (33,609 compounds), 240 cell line contexts (12 primary & Hematopoietic, Non-cancer, CRISPR cell lines)
- Dose response, ~ 4 patterns
  1. Broadly dose-responsive
  2. Broadly dose-saturated
  3. Selective dose-responsive
  4. Selective dose-saturated

## Data Access
- Migrated to Google BigQuery
- To get a slice, use metadata browser and cmapBQ, however, not of interest for me. (static downloads)
- Tools > Data Library > Expanded CMap LINCS Resource 2020 (CMap2020)
- Transcriptomal Acrivity Score (TAS)
  - Aggregate measure of signature strength (SS) and replicate correlation (CC).
  - $$TAS = \sqrt{SS \cdot max(CC, 0)/978}$$

뒤는 볼 게 없네.. 