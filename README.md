🎬 Movie Recommendation System

A content-based movie recommendation system built using Python, Streamlit, and TMDB API, which suggests similar movies to a user-selected film using cosine similarity on movie feature vectors.

🚀 Features

Recommend top similar movies based on cosine similarity

Display movie posters using the TMDB API

Simple, interactive Streamlit web interface

Efficient pre-computed similarity matrix for fast results

🧠 Tech Stack

Python 3.x

Libraries:

pandas

numpy

scikit-learn

streamlit

requests

pickle (for model persistence)

API: TMDB API


⚙️ How It Works

Each movie is represented as a feature vector (e.g., genre, keywords, cast).

Cosine similarity is computed between all movie pairs.

When a user selects a movie, the system retrieves the top N movies with the highest cosine similarity scores.

Posters are fetched dynamically using the TMDB API.

💻 Installation and Setup

Clone the repository:

git clone https://github.com/yourusername/movie-recommender.git
cd movie-recommender


Create a virtual environment and install dependencies:

python -m venv .venv
.venv\Scripts\activate   # for Windows
pip install -r requirements.txt


Add your TMDB API key in app.py:

api_key = "YOUR_TMDB_API_KEY"


Run the Streamlit app:

streamlit run app.py

🖼️ Example

Input: Avengers: Endgame

Output: Recommended movies → Iron Man, Thor: Ragnarok, Captain America: Civil War, etc.

⚡ Future Improvements

Add hybrid recommendations (content + collaborative filtering)

Include user rating and review integration

Enhance UI/UX with search bar and filters

🧾 License

This project is open-source under the MIT License.
