# Movie Recommendation System with Flask

This project implements a movie recommendation system using Flask, integrating machine learning for movie similarity, user authentication with SQLite database, and data fetching from external APIs.

## Features

- **User Authentication**: Users can sign up, log in, and log out securely.
- **Movie Recommendation**: Based on movie similarity using cosine similarity of plot descriptions.
- **External API Integration**: Fetches movie trailers and user reviews from external sources like The Movie Database (TMDb) and IMDB.
- **Interactive UI**: Provides an interactive UI for users to browse movie recommendations and view details.

## Setup Instructions

1. **Clone the repository**

   ```bash
   git clone <repository_url>
   cd <repository_directory>
   
2.**Install Dependencies**

Ensure you have Python 3.x and pip installed.

pip install -r requirements.txt

3.**Run the Application**


python app.py

**The application will start running locally. Open your browser and go to http://localhost:5000 to view the application.**

## Database Setup

SQLite database (Account.db) is used for user authentication. Tables are created automatically when the application starts if they do not exist.

##API Keys

Replace <your_api_key> in app.py with your actual TMDb API key.

## Usage
-**Sign Up**: Create a new user account to access the recommendation system.
*Log In**: Existing users can log in securely.
**Home Page**: Browse movie suggestions and enter movie titles for recommendations.
**Recommendation** Page: View details of selected movies, including trailers, reviews, and cast information.

## How It Works
The application uses Flask as a web framework to handle user requests and render HTML templates. Here’s an overview of its functionality:

- **Login and Signup**: Users can create accounts securely using a signup form. Existing users can log in with their credentials.
- **Movie Recommendation**: Uses a machine learning model (loaded from nlp_model.pkl) and TF-IDF vectorizer (from tranform.pkl) to recommend movies based on user input.
- **External APIs**: Fetches movie data, trailers, and reviews from external APIs such as TMDb and IMDB to enrich the user experience.
- **Data Persistence**: User account information is stored securely in an SQLite database (Account.db).
  
## Folder Structure
- **pkl/:** Contains serialized machine learning models (nlp_model.pkl, tranform.pkl).
- **datasets/:** Stores CSV data (main_data.csv) used for movie similarity calculations.
- **templates/:** HTML templates for rendering user interfaces (login.html, signup.html, home.html, recommend.html).
- **static/:** Static files like CSS (style.css) and JavaScript (main.js) for front-end functionality.
  
## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to submit an issue or a pull request.

## License
This project is licensed under the MIT License - see the LICENSE file for details.






