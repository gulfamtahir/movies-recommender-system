# Movies Recommender System

This is a content-based movie recommender system that suggests movies to users based on their similarity to other movies using vector cosine similarity. The project uses a dataset from Kaggle and implements content-based filtering to recommend movies.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Models Used](#models-used)
- [Contributing](#contributing)
- [License](#license)

## Introduction
The movie recommender system suggests movies based on their content (such as genres, keywords, cast, etc.) by calculating the cosine similarity between movie vectors. This content-based approach ensures that users receive recommendations based on the attributes of movies they like.

## Features
- **Content-Based Filtering:** Recommends movies based on movie metadata such as genre, cast, crew, and keywords.
- **Cosine Similarity:** Measures the similarity between movie vectors to provide relevant recommendations.
- **Efficient Searching:** Quickly finds and suggests similar movies based on user input.

## Dataset
The dataset used for building the recommender system is from Kaggle and can be accessed at the following link:

[TMDb Movie Metadata Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)

Download the dataset and place it in the `data/` directory of the project.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/movies-recommender-system.git
    cd movies-recommender-system
    ```

2. (Optional) Set up Jupyter Notebook for interactive analysis:
    ```bash
    pip install jupyter notebook
    ```

## Usage

### Running the Recommender System
To get movie recommendations, run the following script:

```bash
python app.py
```

Once the script is running, input the name of a movie, and the system will provide a list of recommended movies based on their similarity.

### Data Preprocessing
The system preprocesses the dataset to extract relevant features like genres, cast, crew, and keywords, which are then transformed into vector representations for calculating cosine similarity.

### Movie Recommendations
The recommender system computes cosine similarity between movies and recommends the top N movies that are most similar to the user’s input movie.

## Models Used

- **Cosine Similarity:** This is the key model used in the project. Cosine similarity is a metric that measures the cosine of the angle between two vectors, allowing us to determine how similar two movies are based on their metadata.

## Contributing
Contributions are welcome! If you have ideas for improvements or find bugs, feel free to open an issue or submit a pull request.

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
