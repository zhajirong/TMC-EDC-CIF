# Breaking the Communication-Accuracy Trade-off: A Sparsified Information Diffusion Framework for Multi-Agent Collaborative Perception

## Overview

This repository contains the supplementary appendix and technical derivations for the paper:

**"Breaking the Communication-Accuracy Trade-off: A Sparsified Information Diffusion Framework for Multi-Agent Collaborative Perception"**

---

## Abstract

This work proposes **EDC-CIF (Event-triggered Diffusion Cubature Information Filter with Covariance Intersection)**, a communication-efficient collaborative perception framework for multi-agent systems, particularly targeting distributed UAV cooperative target tracking under constrained communication resources.

The framework addresses the long-standing trade-off between:

- **Tracking/estimation accuracy**
- **Communication overhead**
- **Computational scalability**

### Key Contributions

- **Error-minimized Event-Triggered Filtering**
  - Reduces redundant transmissions
  - Maintains estimation quality
  - Optimizes filter gain under sparse communication

- **Correlation-aware Diffusion Fusion**
  - Incorporates covariance intersection to mitigate unknown cross-correlations
  - Improves stability and robustness in distributed estimation

- **Sparsified Information Diffusion**
  - Balances local sensing and collaborative reasoning
  - Enables scalable deployment in large observer networks

- **Theoretical Stability Guarantees**
  - Provides stochastic boundedness proofs
  - Ensures mean-square exponential boundedness of estimation errors

---

## Repository Contents

### Appendix Structure

### Appendix A — CKF Algorithm
- Standard Cubature Kalman Filter implementation
- Prediction and update phases
- Baseline nonlinear filtering framework

### Appendix B — Derivation of CIF
- Conversion from covariance form to information form
- Correlation information matrix derivation
- Information contribution vector formulation

### Appendix C — Derivation of ET-CKF
- Event-triggered CKF
- Trigger conditions
- Optimal gain derivation under communication sparsity

### Appendix D — Derivation of ET-CIF
- Event-triggered CIF
- Information matrix approximation
- Non-triggered case derivation

### Appendix E — Stability Analysis
- Mean-square boundedness proof
- Linearized pseudo-system formulation
- Theoretical guarantees for distributed collaborative estimation

### Appendix F — Ablation Studies
- Error-minimized ET filter contribution
- Correlation-aware diffusion contribution
- Dynamic ET baseline comparison

### Appendix G — Additional Baselines
- DEC-CKF comparison
- Communication-performance trade-off analysis

### Appendix H — Full Experimental Results
- Estimation accuracy across:
  - 3 observers
  - 4 observers
  - 8 observers
- Computation efficiency comparisons

### Appendix I — Real-world UAV Experiment
- Manual UAV collaborative tracking
- Position RMSE benchmarks
- Real-world validation

---

## Experimental Highlights

### Performance Improvements
Compared with representative communication-efficient baselines:

- **Lower RMSE**
- **Reduced communication cost**
- **Faster computation**
- **Better scalability with increasing observer numbers**

---

## Core Advantages of EDC-CIF

| Feature | Benefit |
|--------|---------|
| Event-triggered communication | Reduced transmission frequency |
| Information form filtering | Efficient distributed fusion |
| Covariance intersection | Robustness to correlation uncertainty |
| Diffusion strategy | Improved collaborative estimation |
| Stability guarantees | Reliable deployment |

---

## Application Scenarios

- Multi-UAV collaborative target tracking
- Distributed robotics
- Smart sensor networks
- Autonomous vehicle coordination
- Resource-constrained perception systems
- Edge intelligence

---

## Citation

If you use this work, please cite the original paper:

```bibtex
@article{zha2026edccif,
  title={Breaking the Communication-Accuracy Trade-off: A Sparsified Information Diffusion Framework for Multi-Agent Collaborative Perception},
  author={Zha, Jirong and Zhao, Chenyu and Zhou, Nan and Liu, Zhenyu and Sun, Tao and Zhang, Bin and Zhang, Xiaochun and Chen, Xinlei},
  journal={IEEE Transactions on Mobile Computing},
  year={2026}
}
