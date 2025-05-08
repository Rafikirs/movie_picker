# Data Science Project – Movie Picker

> Project created during the bootcamp Data Science & AI of the school Le Wagon as part of a team of 4 people.        
> Availability : The recommendation system is not available online anymore, but you can have a look at it through this presentation video : https://www.youtube.com/watch?v=YYszg2pyiV4

---


## 1. Project choice

- Subject : *As movies fans, we decided to create a movie recommendation system that would allow anyone to input a movie they loved and get recommendations based on it.*
- Data used : *Lots of datasets about movies exist online. We went for a Kaggle dataset from Letterboxd because it was complete enough with few missing data and it contained many movies from all around the world.*


---


## 2. Data preprocessing and features choice

We preprocessed the data very classically, using encoding, imputing, scaling, dropping columns, etc.
For the 1st model we built, we used the movies synopsis.
For the 2d one, we added the languages and genres.


---


## 3. Models used

- We started with a baseline model made using tf-idf on movies synopsis and Nearest Neighbors with a cosine similarity to retrieve recommendations.
- Then we made a more complex model using an auto-encoder supposed to learn the main important aspects of the tf-idf data, movie genre, and movie language. So we used tf-idf, then autoencoder and finally Nearest Neighbors for that one.


---


## 4. Deployment

### API
- Developped with FastAPI
- Allows to make live predictions 

### User interface
- Created with Streamlit
- Interactive demo of the project available at : https://www.youtube.com/watch?v=YYszg2pyiV4 
