# AI Demo - Movie Recommendation System 🎬

## Overview

This repository demonstrates the implementation of a **collaborative filtering movie recommendation system** using Python and machine learning techniques. The project showcases proficiency in data science, machine learning, and recommendation system development through a practical, real-world application.

## 🎯 Project Description

The Movie Recommendation System uses **item-based collaborative filtering** to suggest movies to users based on their historical ratings and the similarities between different movies. The system processes movie metadata and user ratings to generate personalized recommendations using cosine similarity calculations.

### Key Features

- **Data Preprocessing**: One-hot encoding of movie genres and handling missing values
- **Similarity Computation**: Cosine similarity calculations between movies
- **Collaborative Filtering**: Item-based recommendation algorithm
- **Data Visualization**: Heatmaps showing item similarities
- **Model Evaluation**: Train/test split for validation
- **Real Recommendations**: Generates actual movie title recommendations for users

## 🛠️ Skills and Technologies Demonstrated

### Machine Learning & Data Science
- **Collaborative Filtering**: Implementation of item-based recommendation systems
- **Similarity Metrics**: Cosine similarity calculations for recommendation engines
- **Data Preprocessing**: Feature engineering with one-hot encoding for categorical data
- **Matrix Operations**: Sparse matrix handling and efficient computations
- **Model Validation**: Train/test data splitting and evaluation methodologies

### Python Programming & Libraries
- **Data Manipulation**: `pandas` for data analysis and preprocessing
- **Numerical Computing**: `numpy` for mathematical operations and matrix computations
- **Machine Learning**: `scikit-learn` for similarity metrics and preprocessing tools
- **Scientific Computing**: `scipy` for sparse matrix operations
- **Data Visualization**: `matplotlib` for creating informative plots and heatmaps

### Software Engineering
- **Jupyter Notebooks**: Interactive development and documentation
- **Version Control**: Git workflow and repository management
- **Code Organization**: Clean, well-documented Python code
- **Project Structure**: Logical file organization and documentation

## 📁 Project Structure

```
AI_Demo/
├── README.md                 # Project documentation (this file)
├── MovieRecom.ipynb         # Main Jupyter notebook with implementation
├── MovieRecom.pdf           # PDF version of the notebook
├── .gitignore              # Git ignore file for Python projects
├── movies.csv              # Movie metadata (excluded from repo)
└── ratings.csv             # User ratings data (excluded from repo)
```

## 🚀 Getting Started

### Prerequisites

Ensure you have Python 3.7+ installed with the following packages:

```bash
pip install pandas numpy matplotlib scikit-learn scipy jupyter
```

### Required Data Files

The project requires two CSV files (not included in the repository due to size):

1. **movies.csv** - Contains movie metadata with columns:
   - `movieId`: Unique movie identifier
   - `title`: Movie title with release year
   - `genres`: Pipe-separated list of movie genres

2. **ratings.csv** - Contains user ratings with columns:
   - `userId`: Unique user identifier
   - `movieId`: Movie identifier (links to movies.csv)
   - `rating`: User rating (typically 1-5 scale)
   - `timestamp`: Rating timestamp

### Running the Project

1. **Clone the repository:**
   ```bash
   git clone https://github.com/comedianhhh/AI_Demo.git
   cd AI_Demo
   ```

2. **Add the required data files:**
   - Place `movies.csv` and `ratings.csv` in the project root directory
   - These files should follow the MovieLens dataset format

3. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook MovieRecom.ipynb
   ```

4. **Execute the cells sequentially** to see the recommendation system in action

## 📊 Implementation Highlights

### Data Processing Pipeline
1. **Data Loading**: Imports movie and ratings datasets using pandas
2. **Genre Encoding**: Creates one-hot encoding for 18 different movie genres
3. **Matrix Construction**: Builds user-item rating matrices for collaborative filtering
4. **Data Splitting**: Separates data into training (80%) and testing (20%) sets

### Recommendation Algorithm
1. **Similarity Calculation**: Computes cosine similarity between all movie pairs
2. **Prediction Generation**: Uses weighted averages of similar items for rating prediction
3. **Ranking System**: Sorts predictions to generate top-N recommendations
4. **Validation**: Tests recommendations on held-out user data

### Visualization and Analysis
- **Similarity Heatmaps**: Visual representation of item-item similarities
- **Data Exploration**: Statistical analysis of movies and ratings datasets
- **Performance Metrics**: Evaluation of recommendation quality

## 🎬 Sample Output

The system generates personalized movie recommendations such as:

```
Recommendations for user 16:
1. Heat (1995)
2. Craft, The (1996)
3. Long Kiss Goodnight, The (1996)
4. Boot, Das (Boat, The) (1981)
5. Star Trek: First Contact (1996)
6. Star Trek IV: The Voyage Home (1986)
7. Sneakers (1992)
8. Last of the Mohicans, The (1992)
9. Saint, The (1997)
10. Payback (1999)
```

## 🔍 Technical Achievements

- **Scalable Architecture**: Efficient sparse matrix operations for large datasets
- **Algorithm Implementation**: Custom collaborative filtering from scratch
- **Data Engineering**: Robust preprocessing pipeline handling real-world data challenges
- **Performance Optimization**: Memory-efficient computations using scipy sparse matrices
- **Visualization**: Insightful data exploration and results presentation

## 🌟 Learning Outcomes

This project demonstrates proficiency in:
- Building recommendation systems from first principles
- Implementing machine learning algorithms without high-level frameworks
- Working with real-world, messy datasets
- Creating end-to-end machine learning pipelines
- Developing interactive data science notebooks
- Applying mathematical concepts (cosine similarity, matrix operations) in practice

## 📈 Future Enhancements

Potential improvements and extensions:
- **Advanced Algorithms**: Implement matrix factorization techniques (SVD, NMF)
- **Deep Learning**: Explore neural collaborative filtering approaches
- **Evaluation Metrics**: Add RMSE, precision, recall, and coverage metrics
- **Cold Start Problem**: Address new user/item recommendation challenges
- **Hybrid Systems**: Combine collaborative and content-based filtering
- **Real-time Deployment**: Create API endpoints for live recommendations

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

**Note**: This project was developed as a demonstration of machine learning and data science capabilities. The implementation focuses on educational value and showcasing fundamental concepts in recommendation systems.