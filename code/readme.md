# Official Source Code of VulScribeR


## Replication Steps 
0) Clustering Vulnerable samples into 5 clusters -> use kmeans.ipynb
1) Retrieval phase ->  RAG/com/anon/RAG/Main.java
2) Clustered Sampling, Formulation and Generation -> use generation.ipynb
3) Filtering the Generated samples, adding them to Devign dataset, and adding the extra items for keeping the ratio -> data_selection.ipynb
4) Diversity calculation using entropy -> diversity_calculation.ipynb

Finally, (or after step 3) the augmented dataset will be available in ./container_data/train (for Devign and Reveal) and in the form of a jsonl file for training Linevul (step 4 uses the same jsonl file)


# VulScribeR 官方源代码

## 复制步骤
0) 将易受攻击的样本聚类为 5 个簇 -> 使用 kmeans.ipynb
1) 检索阶段 -> RAG/com/anon/RAG/Main.java
2) 聚类采样、制定和生成 -> 使用generation.ipynb
3) 过滤生成的样本，将它们添加到 Devign 数据集，并添加额外项目以保持比例 -> data_selection.ipynb
4) 使用熵计算多样性 ->diversity_calculation.ipynb

最后，（或在步骤 3 之后）增强数据集将在 ./container_data/train（用于 Devign 和 Reveal）中可用，并以 jsonl 文件的形式用于训练 Linevul（步骤 4 使用相同的 jsonl 文件）