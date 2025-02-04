## **Movie Recommendation System**
A content-based and collaborative filtering recommendation system that suggests movies based on user preferences using the **MovieLens dataset**.

### **Project Overview**
This project builds a **Movie Recommendation System** using Python. It leverages **pandas, NumPy, and scikit-learn** to analyze movie ratings and metadata to generate personalized recommendations.

### **Dataset**
The project utilizes the **MovieLens Small Latest Dataset**, which includes:
- `movies.csv` - Contains movie titles and genres.
- `ratings.csv` - Contains user ratings for movies.

The dataset is downloaded directly via:
```python
! curl http://files.grouplens.org/datasets/movielens/ml-latest-small.zip -o ml-latest-small.zip
```

### **Features Implemented**
1. **Data Preprocessing**
   - Reads movie and ratings data.
   - Handles missing values and duplicates.

2. **Exploratory Data Analysis (EDA)**
   - Visualizes ratings distribution.
   - Analyzes most popular movies.

3. **Recommendation Algorithms**
   - **Content-Based Filtering**: Suggests movies based on similarity in genres.
   - **Collaborative Filtering**: Suggests movies based on user ratings (e.g., using cosine similarity or matrix factorization).

4. **User Interaction**
   - Allows users to input their favorite movies and receive recommendations.
   - Filters movies based on genre, ratings, and popularity.

### **Technologies Used**
- Python 🐍
- Pandas
- NumPy
- Scikit-learn
- Matplotlib (for visualization)

### **Installation**
Clone the repository and install dependencies:
```bash
git clone https://github.com/your-username/movie-recommendation-system.git
cd movie-recommendation-system
pip install -r requirements.txt
```

### **How to Run**
1. Run the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
2. Open `Movie Recommendation System.ipynb`
3. Follow the instructions and run the cells.

### **Example Usage**
Input a movie title:
```python
get_movie_recommendations('Inception')
```
Output:
```
Top 5 Recommended Movies:
1. Interstellar
2. The Matrix
3. The Prestige
4. The Dark Knight
5. Memento
```

### **Future Improvements**
- Implement hybrid recommendation (mixing content-based and collaborative filtering).
- Integrate deep learning techniques.
- Deploy as a web app using Flask or Streamlit.
