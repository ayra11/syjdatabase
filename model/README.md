# Social Network Modeling - Karate Club

This project replicates the social network modeling process of Zachary's Karate Club, based on the paper *Social Networks and the Identification of Peer Effects*. It implements the simulation of social relationship changes and causal effect analysis.

## Table of Contents
- [Introduction](#introduction)
- [Dependencies](#dependencies)
- [Data Description](#data-description)
- [Main Features](#main-features)
- [How to Run](#how-to-run)
- [Results Analysis](#results-analysis)

## Introduction
This code uses `networkx` to process social network data and `pandas` and `numpy` for data analysis. Additionally, `statsmodels` is used for regression modeling to explore causal effects in social networks.

## Dependencies
To run this project, install the following Python libraries:
```bash
pip install networkx pandas numpy statsmodels scikit-learn scipy
```

## Data Description
- **karate.gml**: This file stores the social network data of Zachary's Karate Club.
- **Wave 1 & Wave 2**: Represent the initial social relationships and the simulated changes, respectively.

## Main Features
1. **Load Social Network Data**
   - Read the GML file and construct a `networkx` graph.
   - Generate an adjacency matrix and store it as a `pandas` DataFrame.

2. **Simulate Social Network Changes**
   - Copy `Wave 1` and randomly modify 10% of the relationships to form `Wave 2`.
   - Calculate changes in the number of friends.

3. **Social Network Statistical Analysis**
   - Compute average number of friends, standard deviation, minimum, and maximum values.
   - Analyze patterns of newly formed and broken friendships.

4. **Regression Analysis**
   - Use `statsmodels` for regression modeling to examine causal effects in the social network.

## How to Run
1. Download the `karate.gml` file and place it in the designated directory.
2. Run the `karate1.ipynb` Jupyter Notebook.

## Results Analysis
The execution of this code provides:
- Basic structural information of the social network.
- Statistics on social relationship changes between `Wave 1` and `Wave 2`.
- Analysis of friendship change patterns.
- Regression model estimates to explore causal effects in social networks.

This study provides a foundation for social network modeling and can be used for further exploration of peer effects in networks.
