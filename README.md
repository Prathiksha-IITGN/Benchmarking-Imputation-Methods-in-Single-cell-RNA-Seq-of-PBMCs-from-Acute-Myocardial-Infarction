# Benchmarking-Imputation-Methods-in-Single-cell-RNA-Seq-of-PBMCs-from-Acute-Myocardial-Infarction

Overview

This repository contains benchmarking experiments of multiple imputation methods applied to single-cell RNA sequencing (scRNA-seq) data from peripheral blood mononuclear cells (PBMCs) of patients with acute myocardial infarction (AMI). The study evaluates statistical, graph-based, and machine learning methods to assess their ability to recover biologically meaningful gene expression patterns under different dropout scenarios.

Background

Acute myocardial infarction (AMI) triggers immune cell mobilization and inflammatory responses, which can be captured by scRNA-seq. However, dropout events create sparse and noisy data, complicating biological interpretation. Accurate imputation of missing values is critical for preserving immune signatures and ensuring biologically faithful results.

Methods

We benchmarked the following imputation methods:

- MAGIC – graph-based diffusion denoising 

- IterativeImputer – multivariate feature prediction 

- KNNImputer – nearest-neighbor based filling 

- Mean Imputation – baseline replacement with gene-wise average 

- SoftImpute – matrix completion via low-rank approximation 

- GAN-based Imputation (scIGANs) – deep learning with adversarial networks 
Installation


Results Summary

- GAN-based methods best captured global gene expression and regulatory patterns.

- SoftImpute excelled in preserving cell-type markers and clustering fidelity.

- MAGIC produced inflated silhouette scores but risked oversmoothing.

- KNN and Mean imputation were less effective and often distorted biological signals

