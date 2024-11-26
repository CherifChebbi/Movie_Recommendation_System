# **Movie Recommendation System Using Machine Learning**

## **Overview**
This project is a **Movie Recommendation System** built using machine learning techniques. It recommends movies based on their similarity to a user's favorite movie. By leveraging metadata such as genres, keywords, tagline, cast, and director, the system computes content-based similarity scores to suggest movies that align with user preferences.

---

## **Features**
- **Content-Based Recommendations**: Suggests movies similar to a user's input based on their metadata.
- **TF-IDF Vectorization**: Converts textual features into numerical vectors for similarity computation.
- **Cosine Similarity**: Measures similarity between movies using feature vectors.
- **Dynamic User Input**: Accepts a user's favorite movie title and provides personalized recommendations.
- **Scalable Design**: Optimized to handle large datasets efficiently.

---

## **Dataset**
The dataset (`movies.csv`) includes the following attributes:
- **Title**: Movie name (used for input and recommendations).
- **Genres**: Categories such as Action, Adventure, Drama, etc.
- **Keywords**: Keywords describing the movie's storyline.
- **Cast**: List of main actors.
- **Director**: Name of the movie's director.
- **Tagline**: A short slogan or promotional line.
- **Overview**: A brief description of the movie.
- **Runtime**: Duration of the movie in minutes.
- **Vote Average**: Average user rating.
- **Popularity**: Popularity score based on user engagement.

  ---

## **How It Works**
1. **Data Preprocessing**:
   - Fill missing values in `genres`, `keywords`, `tagline`, `cast`, and `director` with empty strings.
   - Combine these features into a single string for each movie.

2. **Feature Engineering**:
   - Use **TF-IDF Vectorization** to convert textual data into numerical feature vectors.

3. **Similarity Calculation**:
   - Compute **Cosine Similarity** between feature vectors to identify similar movies.

4. **Recommendations**:
   - Take user input for a favorite movie title.
   - Find the closest matching title in the dataset.
   - Recommend the top 30 most similar movies.

---

## **Technologies Used**
- **Python**: Core programming language.
- **Pandas**: For data manipulation.
- **NumPy**: For numerical operations.
- **scikit-learn**: For TF-IDF vectorization and similarity calculations.
- **difflib**: For finding close matches to user input.

---
