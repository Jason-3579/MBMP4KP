# MBMP4KP

**MBMP4KP: A Multi-Behavior and Meta-Path Learning Model for Knowledge Point Recommendation**

## Overview

MBMP4KP is a research project for personalized knowledge point recommendation in online education. It investigates how multiple types of learning behavior and heterogeneous semantic relations can be represented and combined for recommendation.

The proposed framework:

- Organizes learner interactions into four behavior categories: **Enter**, **Learn**, **Mark**, and **Submit**.
- Represents each retained interaction as a **behavior-instance node** connected to its learner and target learning resource in a heterogeneous educational knowledge graph.
- Uses predefined **meta-paths** to model higher-order relations among learners, behavior instances, learning resources, and knowledge points.
- Learns complementary representations through **meta-path random walks** and a **meta-path classification view**, then fuses the two views for knowledge point recommendation.

## Datasets

The study uses the following publicly available datasets:

- [MOOCCube](https://github.com/thukg/MOOCCube)
- [MOOCCubeX](https://github.com/THU-KEG/MOOCCubeX)

Please consult the original dataset repositories for their access conditions and applicable licenses. This repository does not claim ownership of the original datasets.

## Repository organization

The repository contains directories for project components such as `src/mbmp4kp/`, `configs/`, `scripts/`, `experiments/`, `baselines/`, `data/`, `results/`, and `docs/`.

The presence of a directory does not necessarily mean its contents are complete or ready for reproduction.

## Code and experimental data availability

This repository is the designated location for MBMP4KP project materials.

The processed experimental data, complete reproducibility instructions, and research source code are being reviewed and organized for public release. Availability will be updated here as materials are released.

**Current status:** Do not assume that the repository already contains all data, trained models, or scripts required to reproduce the reported results.

## Citation

The accompanying manuscript is being prepared for submission. Bibliographic citation details will be added if and when a citable version becomes available.

## Questions

For questions about publicly available materials, please use this repository's [Issues](https://github.com/Jason-3579/MBMP4KP/issues) page.
