# 📊 AI-Powered Job Skills Prediction Engine

This repository contains a data science project that predicts job skills based on job titles and descriptions. The project demonstrates a complete data pipeline, from raw data extraction and preprocessing to building a recommendation model using vector embeddings and similarity search.

The core of this project is its ability to provide accurate skill recommendations even with noisy, real-world data, making it a powerful tool for job seekers, recruiters, and hiring managers.

## 📁 Repository Structure

* `job_data_extraction.ipynb`: This notebook contains the code for fetching raw job data from various sources (e.g., Upwork, LinkedIn).

* `dataframe_creation.ipynb`: This notebook processes the raw JSON data and combines it into a clean, unified Pandas DataFrame.

* `data_preprocessing.ipynb`: This notebook cleans and prepares the combined data for modeling. This includes handling missing values and ensuring consistent data types.

* `predicting_skills_from_job_description.ipynb`: This is the main analysis notebook. It uses a pre-trained embedding model to convert job titles into numerical vectors and performs a similarity search to find the most relevant jobs and predict skills.

* `requirements.txt`: Lists all the necessary Python libraries for this project.

## ✨ Key Features

* **End-to-End Pipeline**: A complete workflow, from raw data to a functional prediction model.

* **Vector-Based Similarity**: Leverages modern vector embedding models to semantically understand job titles. This approach is highly effective and more robust than traditional keyword-based methods.

* **Flexible Data Sources**: Designed to handle and merge data from multiple, disparate sources.

* **Practical Application**: Solves a real-world problem by providing actionable skill recommendations.

## 🚀 Getting Started

To get started with this project, you'll need to set up your Python environment and download the required AI model.

### Prerequisites

You must have [Ollama](https://ollama.com/) installed and running locally to use the embedding model.

Run the following command in your terminal to download the necessary model:
```
ollama pull nomic-embed-text
```

### Installation

Install the required Python packages using the `requirements.txt` file.

```
pip install -r requirements.txt
```

### Usage

1. Place your raw job data files in the repository directory.

2. Run the Jupyter notebooks in the following order:

   1. `job_data_extraction.ipynb`

   2. `dataframe_creation.ipynb`

   3. `data_preprocessing.ipynb`

   4. `predicting_skills_from_job_description.ipynb`

3. The final notebook will provide skill predictions for a given job title. You can easily modify the input job title to test different queries.
