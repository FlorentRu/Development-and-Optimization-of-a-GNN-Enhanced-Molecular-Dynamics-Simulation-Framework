# Development and Optimization of a GNN Enhanced Molecular Dynamics Simulation Framework

The goal is to develop a framework that integrates Graph Neural Networks to predict interatomic forces in molecular systems, thereby accelerating Molecular Dynamics simulations without compromising accuracy. This repository contains code and resources for developing a Graph Neural Network (GNN) enhanced Molecular Dynamics (MD) simulation framework using PyTorch and OpenMM. In this project we will integrate machine learning models into MD simulations to predict interatomic forces and potential energies more accurately and efficiently.

## Installation

- Prerequisites
- Python 3.12.4
- NVIDIA GPU with CUDA support (for GPU acceleration)
- Conda (recommended for environment management)


## Table of Contents:

- Introduction
- Project Overview
- Features
- Installation
- Dataset Preparation
- Model Architecture
- Training the Model
- Integration with OpenMM
- Performance Optimization
- Results
- Usage
- Contributing
- License
- References

# Introduction

Traditional molecular dynamics simulations rely on predefined force fields, which may not capture all the quantum mechanical effects necessary for accurate modeling of complex molecular systems. By leveraging GNNs, we aim to learn interatomic potentials directly from quantum mechanical data, enabling simulations that are both accurate and computationally efficient.

# Overview
This project is divided into multiple parts:

## 1. Dataset Preparation and GNN Model Development

- Collect and preprocess molecular data using the QM9 dataset.
- Implement a GNN model to predict molecular energies.
  
## 2. Extending the Model to Predict Forces

- Modify the GNN to predict interatomic forces.
- Train the model on appropriate datasets.
  
## 3. Integration with OpenMM

Develop a custom force provider in OpenMM using the trained GNN.
Run MD simulations using the GNN-based force field.

## 4. Performance Optimization

Profile and optimize the simulation framework.
Implement parallelism strategies and GPU acceleration.

## 5. Validation and Analysis

Validate simulation results against benchmarks.
Analyze performance improvements and accuracy.

# Features

## Graph Neural Network Implementation:

- Customizable GNN architecture using PyTorch Geometric.
- Predicts molecular energies and interatomic forces.

## Integration with OpenMM:

- Seamless integration of the GNN model into MD simulations.
- Supports custom force calculations during simulations.

## Performance Optimization:

- Utilizes GPU acceleration and parallel computing.
- Optimized for large-scale simulations.

## Comprehensive Documentation:

- Detailed instructions and explanations.
- Includes examples and tutorials.

## Install Dependencies

- PyTorch and CUDA
#### conda install pytorch torchvision torchaudio cudatoolkit=11.3 -c pytorch

## PyTorch Geometric and Related Libraries

#### conda install pyg -c pyg -c conda-forge

- RDKit
#### conda install -c conda-forge rdkit

- OpenMM
#### conda install -c conda-forge openmm

## Data Preprocessing

- One-Hot Encoding of Atomic Numbers
- Calculation of Edge Attributes (Interatomic Distances)

## Dataset Splitting

## Model Architecture

### MPNN Model Implementation

- Node and Edge Embeddings
- Message Passing Layers
- Update Functions
- Readout Layer

## Training the Model

### Setup
### Training loop

## Results
### Training and Validation Loss Curves
### Model Evaluation on Test Set

## Integration with OpenMM

In the next phase, we will:

- Extend the model to predict forces.
- Develop a custom force provider in OpenMM.
- Run MD simulations using the GNN-based force field

## Performance Optimization

Future steps include:

- Profiling the model and simulation performance.
- Implementing parallelism strategies.
- Optimizing GPU utilization.




