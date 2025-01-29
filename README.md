# Game of Thrones Personality Matcher

## Overview
This is a **Game of Thrones Personality Matcher** web application built using **Streamlit**. The app allows users to select a character from the Game of Thrones universe and find the closest matching character based on personality similarities.

## Features
- Users can select a character from a dropdown list.
- The app calculates the closest personality match using the **t-SNE algorithm**.
- Images of both the selected character and their closest match are displayed.
- The app fetches character images from an external API (**thronesapi.com**).

## Technologies Used
- **Python**: The core programming language used for the application.
- **Streamlit**: A framework for building interactive web applications.
- **NumPy**: Used for numerical calculations and distance computation.
- **Pickle**: Used to load preprocessed data.
- **Requests**: Used to fetch data from an external API.

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/got-personality-matcher.git
   cd got-personality-matcher
   ```
2. Install the required dependencies:
   ```sh
   pip install streamlit numpy requests pickle5
   ```
3. Run the Streamlit app:
   ```sh
   streamlit run app.py
   ```

## How It Works
1. The app loads a dataset containing personality vectors of Game of Thrones characters.
2. The user selects a character from a dropdown list.
3. The app computes the closest match using **Euclidean distance**.
4. Images of both the selected character and the closest match are displayed.

## Data Source
- **Character Data**: Loaded from a preprocessed pickle file (`data.pkl`).
- **Character Images**: Fetched from [ThronesAPI](https://thronesapi.com/).

## Example Output
Upon selecting a character, the app displays:
- The selected character's name and image.
- The closest matching character's name and image.

