# NeuMF Repro Eval

This project reproduces and analyzes the **Neural Collaborative Filtering (NeuMF)** model using the **MovieLens 100K** dataset, as part of a university assignment. It focuses on evaluating NeuMF under various settings and comparing it to **Non-negative Matrix Factorization (NMF)** for top-K recommendation tasks.

>  The core NeuMF model is taken from an open-source implementation. This project focuses on **experimentation**, **evaluation**, and **comparative analysis**, not on building the model from scratch.

---

##  What’s Included

- Experiments on NeuMF with:
  - Varying number of MLP layers (1 to 3)
  - With and without pretraining
  - Varying number of negative samples
- Evaluation metrics:
  - HR@K (Hit Ratio)
  - NDCG@K (Normalized Discounted Cumulative Gain)
- Training curves:
  - Loss, HR@10, NDCG@10 vs. epochs
- NMF implementation adapted for top-K recommendation using `scikit-learn`
- Final comparison of NeuMF vs. NMF:
  - HR@10, NDCG@10, model parameter counts

---

##  Dataset Info

- **MovieLens 100K (u.data)**
- 100,000 interactions from 943 users and 1682 items
- Format: `user_id | item_id | rating | timestamp`
- Only implicit feedback used (ratings binarized)
- Timestamp ignored

##  References

- He, Xiangnan, et al. “Neural Collaborative Filtering.” *Proceedings of the 26th International Conference on World Wide Web*, 2017. [arXiv:1708.05031](https://arxiv.org/abs/1708.05031)
- Official NeuMF implementation (PyTorch): [hexiangnan/neural_collaborative_filtering](https://github.com/hexiangnan/neural_collaborative_filtering)
- MovieLens 100K Dataset: [GroupLens Research](https://grouplens.org/datasets/movielens/)
- Scikit-learn’s NMF module: [https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.NMF.html](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.NMF.html)

