# Hackwise 2.0 — Chihuahua vs Muffin Challenge
## Team: Pixel Pirates | KVGCE

### Problem Found in Dataset
- Dataset was heavily imbalanced: only 50 Chihuahua and 50 Muffin images
- Several mislabeled images (Chihuahua labeled as Muffin and vice versa)
- Some blurry, low-quality, and visually ambiguous images confused the model
- Background bias: model was learning background context instead of the object

### What We Fixed
- Identified and corrected mislabeled samples using 3LC per-sample metrics
- Removed blurry and low-quality images from the dataset
- Used embedding visualization to find confusing clusters and outliers
- Adjusted sample weights — reduced weight of ambiguous images
- Cleaned dataset versions tracked using 3LC Tables and Runs

### Results
| Stage | Accuracy |
|-------|----------|
| Baseline (original dataset) | 76.10% |
| After label fixes + cleaning | ~85% |
| Final (best validation) | **91.50%** |

### Tools Used
- 3LC Platform (https://3lc.ai) — dataset versioning, embeddings, runs
- Python

### Team
- **Team Leader:** Shresta
- **Members:** Thrisha, Preethika
- **College:** KVG College of Engineering, Sullia
- **Event:** Hackwise 2.0 — March 14, 2026