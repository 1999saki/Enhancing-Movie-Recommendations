# Movie Recommendation System: A Comparative Study of Collaborative Filtering and Hybrid Approaches

This project aims to compare the performance of recommender systems using two different approaches: **Collaborative Filtering (Matrix Factorization)** and **Hybrid Recommender Systems**, which combine collaborative filtering, content-based filtering, and sentiment analysis. The MovieLens dataset and Twitter sentiment data are used to evaluate the performance of these models. The results indicate that the hybrid model, which incorporates sentiment scores, performs better than traditional collaborative filtering methods in certain cases.

## Project Contributors:
- **Avishek Ananda Jha**
- **Keerthana Amalanathan Valarmathi**
- **Sai Kiran Pilli**
- **Priyanka Kothapalli**

### Technologies Used:
- **Matrix Factorization (Collaborative Filtering)** using PyTorch.
- **Hybrid Recommender System** integrating collaborative filtering, content-based filtering, and sentiment analysis.
- **Sentiment Analysis** using Twitter data and the VADER sentiment analysis tool.
- **MovieLens Dataset** for user-item interactions and movie ratings.
  
### Key Features:
- **Collaborative Filtering with Matrix Factorization:** Decomposes the user-item interaction matrix into latent factors for improved predictions.
- **Hybrid Recommender System:** Combines collaborative filtering with content-based filtering and sentiment scores derived from movie-related tweets.
- **Neural Embedding Layer:** Utilizes user, item, genre, and sentiment embeddings to improve recommendation accuracy.
- **Sentiment Score Calculation:** Sentiment scores from Twitter are used as an additional feature in the hybrid recommender system to enhance recommendations.
  
### Datasets:
- **MovieLens Dataset (u.data, u.item):** Contains 100,000 movie ratings from 943 users on 1,682 movies.
- **Twitter Sentiment Data:** Contains sentiment scores for each movie based on related tweets.

### Methodology:
1. **Data Preprocessing:** Combining MovieLens ratings, genres, and sentiment scores.
2. **Model Training:** Training the Collaborative Filtering (Matrix Factorization) and Hybrid Recommender models.
3. **Evaluation Metrics:** RMSE, MAE, Precision, Recall, and F1-Score were used to evaluate the models.

### Results:
- **Collaborative Filtering:** Achieved better accuracy with RMSE ranging from 0.68 to 1.03 depending on the latent sizes.
- **Hybrid Model:** Showed potential but underperformed with an RMSE between 1.01 to 4.93, highlighting areas for improvement.

### Visualizations:
- Plots for RMSE, MAE, and other evaluation metrics.
- Performance comparison for top-10 and top-20 movie recommendations.
- Loss tracking over 10 epochs for both models.

### Conclusion:
The hybrid approach, while theoretically sound, requires further refinement to outperform the Matrix Factorization method. Future work could explore better integration techniques and additional features to improve the hybrid model's performance.

---

### References:
- He et al. (2017). Neural Collaborative Filtering. *Proceedings of the 26th International Conference on the World Wide Web*.
- Rendle et al. (2012). Factorization Machines. *ACM Transactions on Intelligent Systems and Technology*.
- Burke (2002). Hybrid Recommender Systems. *User Modeling and User-Adapted Interaction*.
