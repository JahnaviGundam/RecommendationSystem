# RecommendationSystem
This is a Content-Based Recommender System that suggests similar movies to a user-selected title
## Dataset
Source: Kaggle - TMDB 5000 Movie Dataset

Files Used:

tmdb_5000_movies.csv

tmdb_5000_credits.csv

## Methodology
### Data Preprocessing:

Merged movies and credits datasets on the title.

Selected important features: genres, keywords, overview, cast, crew.

Extracted the director and main actors.

Combined selected features into a single text string per movie.

### Text Vectorization:

Applied CountVectorizer to convert the combined text into numerical vectors.

### Similarity Computation:

Calculated cosine similarity between movies using vectorized text.

### Recommendation:

When a user selects a movie, the system returns the top 5 most similar movies based on cosine similarity.

