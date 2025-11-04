# Key Features
- Attention-Aware Fusion between MF and MLP branches for adaptive learning
- Personalized Top-N Movie Recommendations
- Enhanced Diversity, Novelty, and Serendipity using embedding-based metrics
- Interactive Streamlit Deployment Ready for real-time inference

# Tech Stack
- Programming Language - Python
- Libraries - Pandas, NumPy, Matplotlib, Seaborn
- Framework     -     PyTorch
- Model Optimization - AdamW, Early Stopping, Dropout Regularization
- Dashboard     -     Streamlit
- Dataset       -     Movielens 1M

# Model Architecture
1. **Matrix Factorization branch** → captures linear user–item interactions  
2. **MLP branch** → models non-linear interactions with genre embeddings  
3. **Attention Fusion Layer** → adaptively combines MF and MLP representations  
4. **Sigmoid-based output** scaled to a rating range of [1, 5]

# Dataset - Movielens 1M
- 1 million ratings from 6,000 users on 4,000 movies  
- Includes genre
- Preprocessed into user–item–genre tensors for PyTorch

# How Diversity, Novelty and Serendipity works
- Diversity — penalizes similarity among recommended items using cosine distance in embedding space
- Diversity — penalizes similarity among recommended items using cosine distance in embedding space
- Serendipity — combines diversity and novelty for unexpected yet relevant recommendations

# References
- He et al., Neural Collaborative Filtering
- Chen et al., Attentive Collaborative Filtering: Multimedia Recommendation with Item- and Component-level Attention
- MovieLens Dataset — GroupLens Research
