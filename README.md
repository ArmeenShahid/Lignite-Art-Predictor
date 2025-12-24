Lignite-Art-Predictor
This application predicts the number of expected likes and what time to post content at my art account named "Lignite Art." This utilizes a multiple linear regression model for predicting the numeric values. The dataset includes the number of likes, the number of views, the number of hashtags, the type of post, and the category of post.
Lignite Art Engagement Predictor

The goal is to help decide what type of content to post (Digital Art vs Sketches) and when to post it to maximize engagement.


Project Overview

Social media engagement depends on multiple factors, such as:

Content type
Posting time
Hashtag usage
Reach / views

This project applies Multiple Linear Regression to historical Instagram post data from Lignite Art to:

Predict the number of likes a post may receive
Recommend the optimal posting hour
Provide a simple and aesthetic Flask-based user interface



Machine Learning Concept Used

Linear Regression

Type: Supervised Learning (Regression)
Why: Likes and posting time are continuous numeric values
Model: Multiple Linear Regression

Feature Engineering

Converted time into hours
One-hot encoded categorical features (Digital Art / Sketches)

Features Used

| Feature       | Description                              |
| ------------- | ---------------------------------------- |
| category      | Post type (Digital Art / Sketches)       |
| hashtag_count | Number of hashtags used                  |
| views         | Expected post reach                      |
| hour          | Posting hour (target for recommendation) |
| likes         | Engagement count (main target variable)  |

What the Model Predicts

1. Expected Likes (Primary Target)
2. Best Posting Time (Hour) (Secondary Target)

The model helps answer:
“If I post Digital Art or Sketches today, how many likes can I expect, and when should I post?”







Project Structure

lignite_flask_app/
│
├── app.py
├── lignite_data_linearregression.xlsx
│
├── static/
│   ├── lignite_art_logo.jpg
│   └── style.css
│
└── templates/
    └── index.html
```

---

 How to Run the Project

 1️⃣ Install Dependencies

```bash
pip install flask pandas scikit-learn openpyxl
```

2️⃣ Run Flask App

```bash
python app.py
```

 3️⃣ Open in Browser

```
http://127.0.0.1:5000
```

---

User Interface

Brand-aligned color scheme (Grey, White, Maroon)
Logo support for Lignite Art
Simple and intuitive form inputs
Clean output display for predictions


Example Output

❤️ Expected Likes: 19
⏰ Best Posting Time: 21:00
🔥 Trending Category: Sketches (based on prediction)

Future Improvements

Add confidence intervals for predictions
Compare Digital Art vs Sketches side-by-side
Include reels vs static posts
Visualize engagement trends using charts
Deploy on cloud (Render / Railway / AWS)



Author

Armeen Shahid
AI / ML Enthusiast | Designer | Researcher
Project built as part of an AI Engineer learning roadmap



Why This Project Matters

This project demonstrates:

Practical Application of Linear Regression
Feature encoding & preprocessing
ML-to-Web integration using Flask
Real-world decision-making use case for creators




