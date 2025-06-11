# STEP: Spatial Temporal Graph Convolutional Networks for Emotion Perception from Gaits

This is the official implementation of the paper:  
**[STEP: Spatial Temporal Graph Convolutional Networks for Emotion Perception from Gaits](https://aaai.org/ojs/index.php/AAAI/article/view/5490)**

### 🔗 Emotion-Gait Dataset

We have also released the Emotion-Gait dataset, which is available for download here:  
👉 [https://go.umd.edu/emotion-gait](https://go.umd.edu/emotion-gait)

---
🏷️ Labels Used
In this implementation, we work with two types of label sets:

Original labels: Emotion annotations provided with the official Emotion-Gait dataset.

Re-assigned labels: Labels that are manually or automatically re-generated based on alternative criteria or annotation methods.

These two sets are used to compare performance and study the robustness of emotion classification under different labeling strategies.

---
### 📁 Repository Structure

- `generator_cvae/` — The conditional VAE-based generator.
- `classifier_stgcn_real_only/` — Baseline classifier using only the 342 real gaits.
- `classifier_stgcn_real_and_synth/` — Baseline classifier using both 342 real and N synthetic gaits.
- `classifier_hybrid/` — Hybrid classifier using both deep and physiologically-motivated features.
- `compute_aff_features/` — Scripts to compute affective features from 16-joint pose sequences.
---
If you find our work useful, please cite it using the following format:

```bibtex
@inproceedings{bhattacharya2020step,
  author    = {Bhattacharya, Uttaran and Mittal, Trisha and Chandra, Rohan and Randhavane, Tanmay and Bera, Aniket and Manocha, Dinesh},
  title     = {STEP: Spatial Temporal Graph Convolutional Networks for Emotion Perception from Gaits},
  booktitle = {Proceedings of the Thirty-Fourth AAAI Conference on Artificial Intelligence},
  year      = {2020},
  pages     = {1342–1350},
  publisher = {AAAI Press},
  series    = {AAAI’20},
  numpages  = {9}
}
