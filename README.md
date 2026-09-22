# RNN-Based Resource Allocation for a Wireless Network

**Samudrala Hareesh** — 621243

## Overview

An RNN model that predicts resource demand in a wireless network over time, framed as a time-series prediction problem, to enable efficient dynamic resource allocation.

## Methodology

- **Model (PyTorch):** Input layer (network state features) → RNN layer (captures temporal dependencies) → fully connected layer (predicts per-user resource allocation)
- **Data:** Synthetic network-state features (e.g., user location, channel quality) with corresponding resource-demand targets; split into train/test sets
- **Training:** MSE loss, Adam optimizer, 50 epochs

## Results

- **Training loss** decreased consistently and converged near zero by ~epoch 20, showing effective learning.
- **Predicted vs. actual resource demand** closely tracked the true trend on test data, confirming the RNN captured the underlying temporal patterns.

## Conclusion

The RNN successfully learned from historical network conditions to predict future resource demand, showing promise for dynamic resource allocation in wireless networks. Future work: extend to more network conditions and validate on real-world data.

## References

1. Zhang & Wang (2019). *Resource allocation for multi-user wireless networks based on RNNs.* IEEE TNNLS.
2. Chen, Li & Yu (2021). *Dynamic resource allocation in cloud computing using RNNs.* FGCS.
3. Kumar & Kumar (2020). *Deep learning-based resource allocation in smart grid.* IEEE Trans. Smart Grid.
4. Zhao & Xu (2020). *RNN-based intelligent resource allocation for IoT applications.* J. Network and Computer Applications.
