# 🎬 Movie Recommendation System using k-Nearest Neighbors (kNN)

This project is a simple **movie recommendation system** built using the **k-Nearest Neighbors (kNN)** algorithm. It takes a random movie (via random index) and recommends a set of similar movies based on user ratings.

---

## 📁 Dataset

The project uses the [MovieLens dataset]([https://www.kaggle.com/datasets/grouplens/movielens-latest-small](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata?resource=download)) from Kaggle:
- `movies.csv` – contains movie titles and genres.
- `ratings.csv` – contains user ratings for movies.

---

## 🛠️ Technologies Used

- **Python**
- **NumPy**
- **Pandas**
- **scikit-learn** (NearestNeighbors)
- **SciPy** (csr_matrix)

---

## 📌 How It Works

1. Loads `movies.csv` and `ratings.csv`.
2. Creates a **user-movie rating matrix** using pivot.
3. Converts the matrix to a **sparse matrix** using `csr_matrix`.
4. Fits the **kNN model** using cosine similarity.
5. Picks a **random movie index** and finds the most similar movies.
6. Prints the list of recommended movie titles.

---

## 📂 Project Structure

📦knn-movie-recommender/
┣ 📄 movies.csv
┣ 📄 ratings.csv
┣ 📄 knnrecommendation.pynb
┣ 📄 README.md

## 📝 Sample Output

Recommendations for Princess Bride, The (1987):

1: Monty Python and the Holy Grail (1975), with distance of 0.368708074092865:
2: Star Wars: Episode V - The Empire Strikes Back (1980), with distance of 0.39714330434799194:
3: Ferris Bueller's Day Off (1986), with distance of 0.39811694622039795:
4: Raiders of the Lost Ark (Indiana Jones and the Raiders of the Lost Ark) (1981), with distance of 0.4048547148704529:
5: Groundhog Day (1993), with distance of 0.4066782593727112:


# 🎬 Movie Dataset Visualization Project

This repository provides a visual analysis of movie data using Python and libraries like **Pandas**, **Matplotlib**, and **Seaborn**. It merges and analyzes two datasets (`movies.csv` and `ratings.csv`) to explore movie ratings, vote counts, and popularity.

---

## 📁 Datasets Used

### ✅ movies.csv
| Column        | Description                         |
|---------------|-------------------------------------|
| `movie_id`    | Unique movie identifier             |
| `title`       | Movie title                         |
| `cast`        | JSON-style string of cast members   |
| `crew`        | JSON-style string of crew members   |

### ✅ ratings.csv
| Column         | Description                          |
|----------------|--------------------------------------|
| `id`           | Corresponds to `movie_id`            |
| `title`        | Movie title                          |
| `vote_average` | Average rating from users            |
| `vote_count`   | Number of votes received             |
| ...            | Other metadata like `budget`, `genres`, etc. |

---

## 📊 Visualizations

### 1. **Top 10 Highest Rated Movies**
Bar plot of movies sorted by average rating (`vote_average`).

### 2. **Vote Count vs Average Rating**
Scatter plot showing how vote count correlates with rating.

### 3. **Top 5 Movies by Vote Count**
Pie chart representing the top 5 movies with the highest number of votes.

---

## 🧰 Tech Stack

- Python 3.x
- Pandas
- Matplotlib
- Seaborn

---
