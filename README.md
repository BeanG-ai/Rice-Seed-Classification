Dưới đây là mẫu file README cho dự án phân loại hạt giống gạo sử dụng các thuật toán học máy (Machine Learning). 

---

# Rice Seed Classification

This project focuses on classifying rice seed images into distinct varieties using machine learning algorithms. The goal is to develop an accurate model capable of distinguishing between different types of rice seeds based on visual characteristics.

## Table of Contents

1. [Overview](#overview)
2. [Dataset](#dataset)
3. [Model Architecture](#model-architecture)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Results](#results)
7. [Contributing](#contributing)
8. [License](#license)

## Overview

 This study aims to enhance the classification accuracy of rice seed images using stacking and
 bagging techniques with 52 basic features. Various machine learning methods were employed,
 achieving high accuracy rates: Random Forest at 96.03% and Support Vector Machine at 96.44%,
 etc. Additionally, an Artificial Neural Network (ANN) was implemented, achieving an accuracy
 of 97.45%. Our proposed approach, which combines these techniques through stacking, resulted
 in an average accuracy of 97.91%. This significant improvement demonstrates the effectiveness of
 stacking, bagging in enhancing rice seed classification performance.
## Dataset

 Six commonly cultivated rice seed varieties in Northern Vietnam—BC-15, Hương thơm 1, Nếp-87, Q
5, Thiên ưu-8, and Xi-23—were examined. These rice seeds were sourced from a production company
 where the varieties were cultivated and harvested under specific conditions to meet standard rice seed
 production requirements. The sampling was conducted in the Thaibinh and Hanoi regions in Northern
 Vietnam.
| Rice Variety     | Number of Individual Rice Seed Images |
|------------------|---------------------------------------|
| BC-15            | 3680                                  |
| Hương thơm 1     | 4152                                  |
| Nếp-87           | 2877                                  |
| Q-5              | 3019                                  |
| Thiên ưu-8       | 2011                                  |
| Xi-23            | 4152                                  |



## Model Architecture

The project utilizes several architectures to classify rice seeds, including:
1. **Feature extraction:** Basic descriptor, GIST descriptor, SIFT Descriptor, HOG Descriptor, LBP Descriptor and GLCM Descriptor.
2. **Model:** using models such as Support vector machine, K-Nearest Neighbors, Random-Forest, Logistic Regression and Artificial Neural Networks (ANN).
3. **Proposed mode** Bagging and Stacking.


## Results
### Table: Performance Comparison of Different Models Using 52 Basic Features
| Seed            | KNN F | KNN Acc | SVM F | SVM Acc | RF F  | RF Acc | Logistic Regression F | Logistic Regression Acc | ANN F  | ANN Acc |
|-----------------|-------|---------|-------|---------|-------|--------|------------------------|-------------------------|--------|---------|
| BC-15           | 89.22% | 88.22% | 92.16% | 91.93% | 91.94% | 91.93% | 90.84%                 | 90.61%                  | 94.81% | 94.81%  |
| Hương thơm 1    | 95.60% | 95.33% | 97.78% | 97.66% | 97.44% | 97.37% | 97.42%                 | 97.30%                  | 98.54% | 98.54%  |
| Nếp-87          | 95.93% | 95.89% | 98.10% | 98.10% | 97.40% | 97.47% | 98.21%                 | 98.21%                  | 98.21% | 98.21%  |
| Q-5             | 93.45% | 92.96% | 96.99% | 96.88% | 95.09% | 95.17% | 94.98%                 | 94.77%                  | 98.29% | 98.29%  |
| Thiên ưu-8      | 96.04% | 95.92% | 98.05% | 98.04% | 97.50% | 97.43% | 98.65%                 | 98.64%                  | 98.04% | 98.04%  |
| Xi-23           | 94.01% | 93.20% | 96.45% | 96.05% | 96.90% | 96.78% | 94.22%                 | 93.57%                  | 96.78% | 96.78%  |
| **Average**     | 94.04% | 93.59% | 96.59% | 96.44% | 96.06% | 96.03% | 95.72%                 | 95.52%                  | 97.45% | 97.45%  |


### Table: Performance Metrics Using 52 Features

|               | **Bagging (52 features)**                   |             |             |             |             | **Stacking (52 features)**                   |             |             |             |
|---------------|---------------------------------------------|-------------|-------------|-------------|-------------|----------------------------------------------|-------------|-------------|-------------|
| Seed          | P                                           | R           | F           | Acc         | P           | R           | F           | Acc         |
| BC-15         | 93.42%                                      | 93.28%      | 93.32%      | 93.33%      | 95.31%      | 95.30%      | 95.30%      | 95.30%      |
| Hương thơm 1  | 98.17%                                      | 98.17%      | 98.17%      | 98.18%      | 98.61%      | 98.61%      | 98.61%      | 98.61%      |
| Nếp-87        | 98.21%                                      | 98.21%      | 98.21%      | 98.21%      | 98.84%      | 98.84%      | 98.84%      | 98.84%      |
| Q-5           | 97.76%                                      | 97.65%      | 97.68%      | 97.69%      | 98.69%      | 98.69%      | 98.69%      | 98.69%      |
| Thiên ưu-8    | 98.34%                                      | 98.34%      | 98.34%      | 98.34%      | 98.64%      | 98.64%      | 98.64%      | 98.64%      |
| Xi-23         | 96.51%                                      | 96.52%      | 96.56%      | 96.56%      | 97.37%      | 97.37%      | 97.37%      | 97.37%      |
| **Average**   | 97.07%                                      | 97.03%      | 97.04%      | 97.05%      | 97.91%      | 97.91%      | 97.91%      | 97.91%      |


These results highlight the strengths of different architectures in classifying rice seed varieties accurately.

## Contributing

We welcome contributions to enhance the project. Please open an issue to discuss any major changes before submitting a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

--- 

This README provides a comprehensive overview of the project, from setup to results, making it easier for others to understand, install, and potentially contribute. Let me know if you'd like to add or modify any details.
