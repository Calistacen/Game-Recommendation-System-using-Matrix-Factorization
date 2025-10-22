# Game-Recommendation-System-using-Matrix-Factorization
A machine learning project that implements a Collaborative Filtering recommendation engine using Matrix Factorization to predict user ratings for video games.

## Objective & Methodology
To build an accurate and versatile recommendation system model capable of predicting user preferences for video games and filtering results based on specific metadata like Genre, Platform, and Year.

#### Methodology
1. **Collaborative Filtering:** The chosen methodology to predict unknown user-game ratings.
2. **Matrix Factorization**: The core technique, utilizing an optimization method like SGD, to decompose the user-item interaction matrix into latent factor matrices.
3. **Filtering Logic**: Implementing a post-prediction filtering system to allow users to narrow down recommendations by Name, Genre, Platform, and Year of Release.

## Dataset Detail
The project uses a video game dataset containing user interactions and game metadata.
- **Source**: Lecturer provided tsv file
- **Data Type**: Sparse User-Item Interaction Matrix.
- **Features**: Name, Genre, Platform, Year of Release

## Model and Evaluation
The core model is Matrix Factorization for Collaborative Filtering, using cosine similarity on the count vectorized metadata 
The testing went well for all input test and handled wrong input smoothly, successfully recommend relevant games based on the input queries and flexibility to search by multiple features 

## Areas of improvement
1. **Platform Filtering:** Recommendations for Platform: 'PS2' included games from other platforms. Adding stricter filters or weights could improve specificity.
2. **Year Matching:** Recommendations for Year_of_Release included games from nearby years. Implementing exact matches or year bins (e.g., "2000-2005") could improve relevance.
3. **Case Sensitivity:** Queries such as name: 'wii' fail due to case sensitivity. Adding input normalization (e.g., converting all inputs to lowercase) could improve usability.




This project is for educational purposes only.
by Calista.L
