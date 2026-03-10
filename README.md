# A Reproduction and Critique of Kolmogorov-Arnold Networks

This is the repository for the main project of the course _Deep Learning, Advanced Course_ I took during my exchange semester in KTH, together with [@pol-resina](https://github.com/pol-resina) and [@andrelindgren](https://github.com/andrelindgren).

### Abstract:
> This project replicates Kolmogorov-Arnold Networks (KANs), confirming their superior parameter efficiency and adherence to $N^{-4}$ scaling laws in low-complexity tasks. Critically, our reproduction found KANs highly susceptible to overfitting when increasing capacity, displaying U-shaped error curves. In special function approximation, MLPs were significantly more robust, achieving lower test RMSE in 10 out of 15 benchmarks. Finally, KANs successfully demonstrated locality
by avoiding catastrophic forgetting in a 1D problem, but this property failed to generalize to a 2D classification task.

## Repository Structure

```
├── notebooks/                          # Jupyter notebooks containing all experiments
│   ├── toy_functions.ipynb             # Basic KAN vs MLP comparison on toy functions
│   ├── special_functions.ipynb         # Function approximation on special functions
│   ├── reproduce_feynman.ipynb         # Feynman benchmarks (base implementation)
│   ├── reproduce_feynman_2.ipynb       # Additional Feynman benchmark variants
│   ├── reproduce_feynman_cluster.ipynb   # Clustered Feynman experiment analysis
│   ├── reproduce_feynman_cluster2.ipynb  # Extended cluster analysis
│   ├── reproduce_feynman_seed_and_samples.ipynb  # Robustness analysis
│   ├── reproduce_continual_learning.ipynb        # Locality & catastrophic forgetting tests
│   ├── extension_moons_classification_base.ipynb               # 2D classification baseline
│   ├── extension_moons_classification_sequential_class.ipynb   # Sequential class learning
│   ├── extension_moons_classification_sequential_feature.ipynb # Sequential feature learning
│
├── report.pdf         # Detailed project report
├── KAN.pdf            # Original KAN paper
├── LICENSE            # Project license
└── README.md          # This file
```

### Notebook Descriptions

- **Toy Functions**: Simple 1D and 2D function approximation benchmarks comparing KAN and MLP parameter efficiency and scaling laws
- **Special Functions**: Tests KAN and MLP robustness on special function approximation (sine, cosine, Bessel, etc.)
- **Feynman Benchmarks**: Reproduces KAN scalability experiments on 100 symbolic physics equations with varying complexity
- **Continual Learning**: Evaluates KAN's locality property in avoiding catastrophic forgetting in sequential learning tasks
- **Moons Classification**: Extension experiments investigating KAN behavior on 2D classification with different learning schemes
