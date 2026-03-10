# A Reproduction and Critique of Kolmogorov-Arnold Networks

This project replicates Kolmogorov-Arnold Networks (KANs), confirming their
superior parameter efficiency and adherence to N −4
scaling laws in low-complexity
tasks. Critically, our reproduction found KANs highly susceptible to overfitting
when increasing capacity, displaying U-shaped error curves. In special function
approximation, MLPs were significantly more robust, achieving lower test RMSE
in 10 out of 15 benchmarks. Finally, KANs successfully demonstrated locality
by avoiding catastrophic forgetting in a 1D problem, but this property failed to
generalize to a 2D classification task.
