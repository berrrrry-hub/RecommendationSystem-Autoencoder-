# 📊 Autoencoder-Based Collaborative Filtering

## 🚀 Project Overview
This project explores **autoencoder-based collaborative filtering** to build a recommendation system. Compared to traditional **user-based and item-based collaborative filtering**, autoencoders use **deep learning** to capture latent user-item interactions, potentially improving accuracy and learning efficiency.

### **🔄 Common Points with Traditional Collaborative Filtering**
- Uses the **same dataset** (MovieLens dataset with `userId`, `movieId`, `rating`, `timestamp`, `title`, `genres`).
- Aims to **recommend movies** based on past user interactions.
- Evaluates model performance using **RMSE and MAE**.

### **⚡ Key Differences**
| Feature | Traditional Collaborative Filtering | Autoencoder-Based Filtering |
|---------|----------------------------------|----------------------------|
| **Approach** | Memory-based (user-item similarity) | Neural network-based (latent factor extraction) |
| **Scalability** | Struggles with large datasets | More scalable with deep learning |
| **Learning Speed** | Slower, needs more data | Faster, learns efficiently |
| **Overfitting** | Less prone | Higher risk of overfitting |

---

## 📑 Data & Preprocessing
- **Columns:**
  - `userId` – Unique identifier for users
  - `movieId` – Unique identifier for movies
  - `rating` – User-assigned rating for a movie
  - `timestamp` – Time of rating (Unix format)
  - `title` – Movie title
  - `genres` – Genres associated with the movie
- **Data Processing:**
  - Convert ratings matrix into a user-item interaction matrix.
  - Normalize ratings for better training.
  - Train the autoencoder on the matrix to learn user preference patterns.

---

## 🔍 Methodology
1. **Autoencoder Architecture** – Uses a neural network to encode and decode user-item interactions.
2. **Loss Function** – Minimizes reconstruction error to improve recommendation accuracy.
3. **Optimization** – Applies techniques like dropout and batch normalization to enhance performance.

---

## 📊 Results & Insights
- **Model Performance:**
  - **training RMSE:** 0.6088
  - **validating RMSE:** 1.1836
- **Key Observations:**
  - **Autoencoder learns faster** and captures deeper user-item interactions.
  - **More effective** in sparse datasets compared to traditional CF.
  - **Prone to overfitting**, requiring regularization techniques.

📍 **Summary:**
The autoencoder-based method significantly improves learning speed and efficiency, but **overfitting remains a challenge**, requiring careful tuning of hyperparameters and dropout layers.

---

## 📖 Recommended Reading Materials-Autoencoder for recommender systems 
1. Blog post:
   https://towardsdatascience.com/recommendation-system-series-part-6-the-6-variants-of-autoencoders-for-collaborative-filtering-bd7b9eae2ec7

2. Original paper:  
https://users.cecs.anu.edu.au/~akmenon/papers/autorec/autorec-paper.pdf

3. Github implementation:
https://github.com/tuanio/AutoRec


---

## 🔮 Challenges & Future Work
**Challenges:**
- Overfitting due to high model complexity.
- Computational cost increases with deep networks.
- Requires tuning hyperparameters for optimal performance.

**Future Improvements:**
- Implementing **hybrid models** (collaborative + content-based filtering).
- Using **variational autoencoders (VAE)** to handle uncertainty in predictions.
- Experimenting with **attention mechanisms** to improve recommendation diversity.

---

## 👤 Contact & Portfolio
👤 **Jiaxin(Berry) Tian**  
📧 berrytian15@gmail.com  
🔗 https://github.com/berrrrry-hub?tab=repositories
