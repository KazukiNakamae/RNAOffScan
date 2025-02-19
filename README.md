# RNAOffScan Series

**RNAOffScan** is a predictive model for detecting unintended mutagenesis on RNA. In particular, the models focus on predicting off-target editing induced by artificial bio-materials such as Cytocine Base Editor (CBE).

## Available models

| Name | Target | GitHub repository | Hugging Face repository | Description  | Reference |
|------|--------|-------------------|-------------------------|--------------|-----------|
| **RNAOffScan v1**<br>(previously named as STL model) | CBE-induced RNA off-target | 🔗[LINK](https://github.com/KazukiNakamae/STL_model)  | 🔗[LINK](https://huggingface.co/KazukiNakamae/STLmodel) | RNAOffScan v1 is the initial iteration of our machine learning–based system for detecting CBE-induced RNA off-target events. It leverages DNABERT-2 embeddings to classify cytosine-to-uracil (C-to-U) substitutions as either likely CBE-related or background mutations. Serving as a foundational model, RNAOffScan v1 outperforms an ACW motif-based classifier. | [Nakamae *et al*., 2025](https://doi.org/10.3390/ijms26041723) |
| **RNAOffScan v2**<br>(previously named as SNL model) | CBE-induced RNA off-target | 🔗[LINK](https://github.com/KazukiNakamae/SNL_model) | 🔗[LINK](https://huggingface.co/KazukiNakamae/SNLmodel) | RNAOffScan v2 expands upon the capabilities of v1 by incorporating refined hyperparameters, balanced training data, and optimized sequence lengths for improved performance. By capturing broader sequence contexts and implementing enhanced data preprocessing, v2 achieves higher accuracy, precision, recall, and F1 scores than ACW/WCW motif-only classifiers. | [Nakamae *et al*., 2025](https://doi.org/10.3390/ijms26041723)　|
