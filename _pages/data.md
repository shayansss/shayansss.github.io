---
layout: archive
title: "Main Research Data"
permalink: /data/
author_profile: true
---
This page is not complete.

## PMSE: Pointwise Mean Squared Error
-------
  * This repository contains the implementation and dataset files of the "PMSE" metric, described in our *in press* paper at MLIS 2021, entitled "A Pointwise Evaluation Metric to Visualize Errors in Machine Learning Surrogate Models". The exact citation will be added once published.
  PMSE is a simple metric to visualize the correlations between the errors of the machine learning surrogates and corresponding numerical models. Here, we used a simple Keras neural network for surrogate modeling and a finite element method for numerical modeling. The idea is to accelerate the numerical simulation by the surrogate, which is evaluated via the PMSE, and other relevant metrics, during training.
  * Type of data:
        * Machine learning code (mostly by NumPy and Keras on Jupyter Notebook).
        * Finite element model (by Abaqus and its Python script)
        * Visualization (by Abaqus and Matplotlib)
  * Last version is open-sourced at github.com/shayansss/pmse.