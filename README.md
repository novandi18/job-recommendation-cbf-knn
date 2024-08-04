# Skills-Based Job Recommendation System

This project aims to recommend relevant job postings to users based on their skills. The system utilizes a combination of Content-Based Filtering (CBF) and K-Nearest Neighbors (KNN) to provide personalized recommendations.

## How It Works

1. **Content-Based Filtering (CBF):** The system uses TF-IDF to represent user skills and the skills required for each job. Cosine similarity is then calculated to find jobs that are most similar to the user's skills.

2. **K-Nearest Neighbors (KNN):** The top 20 jobs from the CBF results are used to train a KNN model. The KNN model is then used to find jobs that are most similar to the user's skills based on distance in the TF-IDF space.

## Dataset

The dataset used is `lukebarousse/data_jobs` from Hugging Face. This dataset contains information about job postings, including job titles, descriptions, and required skills.

## Model Evaluation

The model is evaluated using Hit Rate and Mean Average Precision (MAP) metrics. Evaluation results indicate that the model performs reasonably well in recommending relevant jobs to users.

## Contribution

Contributions are welcome! Please submit a pull request or open an issue if you find a bug or have a suggestion.

## License

This project is licensed under the MIT License.
