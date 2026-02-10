# Growing Neural Tree Network (GTNN)

We start with a **single parent node** (softmax regression; no hidden layer) and grow a tree by:
1. Training the root on all training data
2. Finding misclassified samples
3. Adding a child node trained only on those misclassified samples
4. Repeating until stopping criteria

We track **train/val/test loss + accuracy** as depth grows.
