---
layout: archive
title: "Main Research Data"
permalink: /data/
author_profile: true
---
This page is not complete.

## PMSE: Pointwise Mean Squared Error
-------
  * **Abstract**: PMSE is a simple metric to visualize the correlations between the errors of the machine learning surrogates and corresponding numerical models. Here, we used a simple Keras neural network for surrogate modeling and a finite element method for numerical modeling. The idea is to accelerate the numerical simulation by the surrogate, which is evaluated via the PMSE, and other relevant metrics, during training.
  * **Type of data**:
      * Machine learning code (mostly by NumPy and Keras on Jupyter Notebook).
      * Finite element model (by Abaqus and its Python script)
      * Visualization (by Abaqus and Matplotlib)
  * **Download link**: Last version is open-sourced at [GitHub](github.com/shayansss/pmse).