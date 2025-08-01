# Social Network Analysis & Recommendation System in Python

## 📖 Project Overview
This project is a comprehensive implementation of a social network analysis tool and a recommendation system, built entirely in Python. It includes features for data cleaning, friend recommendations ("People You May Know"), and content suggestions ("Pages You Might Like"). 

## 🚀 Features
This project is broken down into several key components:

1.  **Data Cleaning & Preparation (`02_Data_Cleaning.ipynb`)**
    * A robust script that cleans raw JSON data.
    * Handles missing user names, removes duplicate friend/page entries, and filters out inactive users.

2.  **Friend Recommendation Engine (`03_People_you_may_know.ipynb`)**
    * Implements a "People You May Know" feature.
    * Suggests new friends to a user based on the number of mutual connections they share.

3.  **Page Recommendation Engine (`04_People_you_might_like.ipynb`)**
    * Implements a "Pages You Might Like" feature.
    * Recommends pages to a user based on the pages liked by other users with similar interests.

## 🛠️ Technology & Libraries
* **Language:** Python
* **Data Format:** JSON
* **Core Libraries:** No external libraries beyond standard Python and JSON were needed.

## 📈 How It Works

### Friend Recommendations
The algorithm works by looking at the friends of a user's direct friends. It counts the number of mutual friends for each person who is not already a direct friend and suggests the people with the highest count.

### Page Recommendations
The page recommendation engine calculates an interest score. It looks at other users who have liked the same pages as the target user. It then suggests new pages based on the collective interests of this group of similar users, weighing pages that are liked by users with more shared interests more heavily.

## ⚡ How to Run
1.  Clone the repository: `git clone ...`
2.  Each feature is contained in its own Jupyter Notebook (`.ipynb`).
3.  Open a notebook (e.g., `03_People_you_may_know.ipynb`) and run the cells to see the output. The code loads its own data file (`03_People_you_may_know_data.json`).
