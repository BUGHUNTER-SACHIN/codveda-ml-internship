# Task 6: Support Vector Machine (SVM) for Classification

## Objective
Implement a Support Vector Machine (SVM) model for binary classification.

## Dataset
Breast Cancer Wisconsin dataset (569 samples, 30 features) — built into scikit-learn
Target: malignant vs benign tumor classification

## Steps Performed
- Scaled all features using StandardScaler (essential for SVM, which is
  distance-based)
- Trained SVM models with both linear and RBF kernels
- Compared performance using accuracy, precision, recall, and AUC
- Visualized decision boundaries for both kernels using PCA (reduced to 2D)

## Results
- Linear Kernel: Accuracy 97.4%, Precision 98.6%, Recall 97.2%, AUC 0.996
- RBF Kernel: Accuracy 98.2%, Precision 98.6%, Recall 98.6%, AUC 0.995

## Key Insight
The RBF kernel achieved higher recall than the linear kernel (98.6% vs
97.2%), meaning it missed fewer actual malignant cases — the clinically
more important metric, since a false negative (missed cancer diagnosis)
is far costlier than a false positive. The linear kernel had a marginally
higher AUC. Both kernels performed excellently overall, indicating the
dataset is close to linearly separable, with RBF's added flexibility
providing a small but meaningful edge in recall.

## Tools Used
Python, pandas, scikit-learn, matplotlib, NumPy

## Files
- `Codveda_Task6_SVM.ipynb` — full notebook with code, kernel comparison,
  and decision boundary visualizations
