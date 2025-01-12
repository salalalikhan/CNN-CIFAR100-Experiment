## Overview
This task delves into the performance analysis of CNN models using the CIFAR-100 dataset under different configurations. It investigates how varying the number of convolutional layers and employing a specific learning rate adjustment method influences the learning behavior of the models.

## Key Results
### **Performance Analysis of Different Configurations**:
| Experiment | Layers Configuration        | Training Accuracy | Test Accuracy |
|------------|-----------------------------|-------------------|---------------|
| 1          | 2 Convolution, 1 Pooling   | 0.15172           | 0.1393        |
| 2          | 2 Convolution, 2 Pooling   | 0.19084           | 0.17          |
| 3          | 3 Convolution, 1 Pooling   | 0.13416           | 0.1225        |
| 4          | 3 Convolution, 2 Pooling   | 0.12298           | 0.118         |

## Key Insights
- **Simpler Models**:
  - The configuration with **2 convolutional layers and 2 pooling layers** showed the best performance.
  - Adding layers beyond this configuration did not yield better results, demonstrating diminishing returns with increased complexity.

- **Impact of RMSprop**:
  - RMSprop effectively adjusted learning rates which aids in faster convergence and particularly for simpler configurations.

- **Hardware Constraints**:
  - Training was limited to 7 epochs due to hardware limitations but extending this could improve performance with careful monitoring.

## Challenges Tackled
1. **Hardware Limitations**:
   - Addressed the constraints of running experiments on limited hardware ensuring the realistic and scalable results.

2. **Overfitting Concerns**:
   - Emphasized the importance of regularization techniques to mitigate overfitting when increasing training epochs.

## Conclusion
This task provided understanding of how CNN configurations, optimizers and training limitations interact to impact model performance. The results highlight the importance of balancing model complexity and generalization ability while optimizing hyperparameters to achieve the best outcomes.
