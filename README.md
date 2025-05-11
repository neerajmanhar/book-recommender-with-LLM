# Book Recommender System using LLMs

This project is a **Semantic Book Recommender System** built using **Large Language Models (LLMs)**. The goal of this system is to recommend books based on natural language queries, classify books by genre, and provide sentiment-based sorting of books. The system uses **vector search**, **text classification**, and **sentiment analysis** to provide accurate and personalized book recommendations.

## Project Overview

The Book Recommender System consists of several key components:

1. **Text Data Cleaning**: The initial step involves cleaning and preparing the book data for further analysis and model training.
2. **Semantic Search**: A vector database is created to allow users to search for books based on the meaning of their queries (e.g., "a book about revenge").
3. **Text Classification**: The system classifies books into genres such as "fiction" and "non-fiction" using zero-shot classification with an LLM.
4. **Sentiment Analysis**: Sentiment analysis is performed on the book descriptions to allow users to sort books based on tone (e.g., suspenseful, joyful, or sad).
5. **Web Application**: A Gradio-based web interface is created for users to easily interact with the recommender system and get personalized book recommendations.

## Features

* **Personalized Book Recommendations**: The system recommends books based on user input and preferences.
* **LLM-based Semantic Search**: The system uses vector search to find books related to a natural language query.
* **Genre Classification**: The books are classified as "fiction" or "non-fiction", allowing users to filter recommendations by genre.
* **Sentiment Sorting**: Books are sorted based on their tone, such as suspense, joy, or sadness.
* **Gradio Dashboard**: The project includes a simple web interface built with Gradio, allowing users to interact with the system easily.

## Technologies Used

* **Python 3.11**
* **LangChain**: For performing tasks like semantic search, text classification, and sentiment analysis.
* **Transformers**: For working with pre-trained LLMs.
* **Gradio**: For building the web application interface.
* **Chroma**: For vector database management and search.
* **Pandas**: For data manipulation.
* **Matplotlib & Seaborn**: For data visualization.
* **python-dotenv**: For managing environment variables (e.g., OpenAI API key).

## Installation & Setup

### Clone the Repository

```bash
git clone https://github.com/neerajmanhar/book-recommender-with-LLM.git
cd book-recommender-with-LLM
```

### Install Dependencies

Create a virtual environment and install the necessary dependencies:

```bash
# Create a virtual environment
python -m venv venv

# Activate the virtual environment
# On Windows
.\venv\Scripts\activate
# On Linux/MacOS
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt
```

### Set Up the OpenAI API Key

To use the OpenAI LLMs, you need to provide your OpenAI API key. Create a `.env` file in the root directory and add your key like this:

```
OPENAI_API_KEY=your-api-key-here
```

### Running the Application

After setting up the dependencies and API key, you can run the project:

```bash
python gradio-dashboard.py
```

This will start the Gradio web interface where you can interact with the Book Recommender System and get personalized book suggestions.

## Data

The dataset used in this project is from **Kaggle**. Instructions for downloading and using the dataset can be found in the repository.

## File Overview

* **`data-exploration.ipynb`**: Preprocessing and cleaning the book data.
* **`vector-search.ipynb`**: Building the vector database for semantic search.
* **`text-classification.ipynb`**: Performing text classification using zero-shot learning.
* **`sentiment-analysis.ipynb`**: Performing sentiment analysis on book descriptions.
* **`gradio-dashboard.py`**: The Gradio web interface for user interaction.

