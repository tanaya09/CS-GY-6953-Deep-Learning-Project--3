# *Deep Learning Adversarial Attack Project*

This repository contains the Jupyter Notebook, generated visualizations, and LaTeX report for our CS-GY 6953 Deep Learning final project on adversarial robustness in image classification.

We evaluate and compare three white-box adversarial attack strategies — *FGSM, **PGD, and **Patch Attack* — using a pretrained *ResNet-34* model on a curated 100-class ImageNet subset. We also assess transferability of the adversarial examples to *DenseNet-121*.

---

## 📊 Summary of Results

| Attack Type | Model         | Top-1 Acc. | Top-5 Acc. | Top-1 Drop | Top-5 Drop |
|-------------|---------------|------------|------------|------------|------------|
| Clean       | ResNet-34     | 76.00%     | 94.20%     | –          | –          |
| FGSM        | ResNet-34     | 3.80%      | 21.00%     | 72.20%     | 73.20%     |
| PGD         | ResNet-34     | 0.00%      | 1.40%      | 76.00%     | 92.80%     |
| Patch       | ResNet-34     | 4.80%      | 34.40%     | 71.20%     | 59.80%     |
| FGSM        | DenseNet-121  | 7.60%      | 27.00%     | 72.40%     | 68.80%     |
| PGD         | DenseNet-121  | 1.80%      | 3.80%      | 78.20%     | 92.00%     |
| Patch       | DenseNet-121  | 8.60%      | 38.40%     | 71.40%     | 57.40%     |

---

## 🔍 Key Highlights

- *FGSM* reveals the model’s vulnerability to fast, single-step perturbations.
- *PGD*, a multi-step iterative attack, causes the most significant performance degradation.
- *Patch attacks* show that small, localized changes can be just as harmful as global noise.
- *Transferability* is high — adversarial examples generated on ResNet-34 also degrade DenseNet-121 performance, showcasing cross-architecture fragility.

---

## 📎 Report

Our detailed project report contains:
- Attack methodology
- Visual samples of clean vs adversarial examples
- Perturbation heatmaps and prediction shifts
- Accuracy drop charts and heatmap comparisons

📄 [Project Report (PDF)]([https://github.com/tanaya09/CS-GY-6953-Deep-Learning-Project--3/blob/main/report/CS6953_Deep_Learning_Project_3__Report.pdf](https://github.com/tanaya09/CS-GY-6953-Deep-Learning-Project--3/blob/main/CS6953_Deep_Learning_Project_3__Report.pdf))

---

## 👥 Contributors

- *Mukesh Durga*
- *Tanaya Pawar*
- *Tejaswini Ojha*

---

## 📘 License

For educational and academic use under NYU Tandon’s CS-GY 6953 Deep Learning course.
