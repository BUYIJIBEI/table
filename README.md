**Table 1**: Classification accuracy and standard error of our method across 3 independent runs on CIFAR-10 and CIFAR-100 using VGG-11 as the teacher and ResNet-18 as the student. Results demonstrate consistency and robustness of the proposed approach.

| Dataset   | Method | Accuracy (%) | Standard Error |
|-----------|--------|---------------|----------------|
| CIFAR-10  | Ours   | 92.50         | ±0.12          |
| CIFAR-100 | Ours   | 72.06         | ±0.08          |

**Table 2**: Sensitivity analysis of the threshold parameter $\tau = Q_p(A(x))$ in Equation (10) across different datasets, with VGG-11 as the teacher network and ResNet-18 as the student network. The results show that the performance of our method remains stable under different $\tau$ values, demonstrating its robustness to the threshold setting.

| Dataset       | $\tau = Q_{0.50}(A(x))$ | $\tau = Q_{0.80}(A(x))$ | $\tau = Q_{0.90}(A(x))$ | $\tau = Q_{0.95}(A(x))$ |
|---------------|--------------------------|--------------------------|--------------------------|--------------------------|
| CIFAR-10      | 92.31                    | 92.39                    | 92.50                    | 92.44                    |
| CIFAR-100     | 71.58                    | 71.86                    | 72.06                    | 71.91                    |

**Table 3**: Ablation experiments on the effectiveness of different thresholding strategies. Evaluated on the CIFAR-100 dataset, with VGG-11 as the teacher network and ResNet-18 as the student network.Validating the effectiveness of our amplitude-guided masking as a thresholding strategy.

| Method                        | Student (%) |
|------------------------------|-------------|
| Random Mask                  | 71.85       |
| High-Frequency Mask          | 71.62       |
| Low-Frequency Mask           | 71.50       |
| Phase Gradient Mask          | 71.87       |
| **Amplitude-Guided Mask (Ours)** | **72.06**   |







