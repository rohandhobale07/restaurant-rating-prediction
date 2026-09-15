                                     🍽️⭐ Restaurant Rating Prediction 🍽️⭐

An end-to-end machine learning web application that predicts prospective customer ratings for restaurants based on business features, deployed as a live, interactive Flask app — not left in a notebook.

📌 Project Overview

This project analyzes Zomato restaurant data using Python and Scikit-Learn to predict customer ratings, then deploys the trained model as a working web interface where a user can input restaurant features and get a live prediction.

🎯 Project Objectives

- Clean and prepare restaurant business data for modeling
- Engineer and encode relevant business features
- Train and compare regression models to predict customer ratings
- Deploy the model as an interactive, user-facing web app

🛠️ Technologies Used

🐍 Python
- Data analysis and modeling

📊 Pandas & NumPy
- Data cleaning and feature preparation

🤖 Scikit-Learn
- Regression modeling

📈 Plotly
- Interactive data visualization

🌐 Flask
- Web app backend and deployment

🎨 HTML / CSS
- Front-end input interface (`index.html`, `style.css`)

🥒 Pickle
- Model serialization for deployment

📁 Dataset

- 🍽️ 23,248 Zomato restaurant records (`Zomato_df.csv`)
- 🔑 8 modeling features: online ordering, table booking, votes, location, restaurant type, cuisines, cost, menu items
- 🎯 Target: customer rating (out of 5)

⚙️ Approach

- Automated missing-data cleaning across the restaurant dataset
- Engineered and encoded business features (online orders, table reservations, pricing, location, vote counts)
- Trained and compared multiple regression algorithms to predict customer rating
- Serialized the best-performing model with Pickle and served it through a Flask backend
- Built a simple HTML/CSS front end so a user can input restaurant features and get a live predicted rating

📈 Model Performance

Trained and benchmarked 3 regression algorithms on a 70/30 train-test split (16,273 train / 6,975 test records):

| Model | R² (Test Data) |
|---|---|
| Linear Regression | 0.228 |
| Random Forest | 0.881 |
| **Extra Trees** | **0.933** |

Extra Trees was the clear winner — a large jump from Linear Regression's 0.228 shows the relationship between restaurant features and rating isn't linear, and tree-based ensembles capture it far better. The Extra Trees model was the one serialized (`model.pkl`) and deployed in the live Flask app.

💡 Key Business Insights

- Online ordering availability significantly boosts customer engagement
- Restaurants with table reservations consistently show higher baseline ratings
- Pricing and location directly influence final rating scores
- Higher vote counts strongly correlate with excellent ratings — popularity and quality reinforce each other

⭐ Project Highlights

🌐 Deployment: Live Flask web app with custom front end

🍽️ Domain: Restaurant/food-service business analytics

🔧 Full Stack: Data cleaning → modeling → deployment → user interface

📊 Records Analyzed: 23,248

🤖 Models Benchmarked: 3 (Linear Regression, Random Forest, Extra Trees)

📈 Best R² (Test Data): 93.3% (Extra Trees)

📉 R² Range: 22.8% – 93.3% across the 3 models



