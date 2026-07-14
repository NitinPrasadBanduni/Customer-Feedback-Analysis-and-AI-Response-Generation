# Customer Feedback Analysis and Automated Response System

## Project Overview

This project was developed as part of the **Imarticus Data Science Internship Assessment (Python Foundations & Generative AI)**.

The objective of this project is to automate the identification of critical customer feedback and generate personalized, empathetic response emails using Generative AI. The solution uses Python for data cleaning and rule-based filtering, followed by the Google Gemini API to create customer support responses for the most urgent reviews.

---

# Objective

The project aims to:

* Clean and preprocess customer review data.
* Identify critical customer reviews using rule-based filtering.
* Extract the most common complaint keywords.
* Generate personalized apology emails using Google Gemini AI.
* Demonstrate the integration of Python and Generative AI for customer support automation.

---

# Dataset

The project uses a customer review dataset containing product reviews and customer ratings.

### Important Columns

* **review_text** – Customer review text
* **rating** – Customer rating (1 to 5 stars)

---

# Technologies Used

* Python
* Pandas
* Collections (Counter)
* Regular Expressions (re)
* Google Gemini API
* Jupyter Notebook

---

# Project Workflow

```
Customer Review Dataset
          │
          ▼
Load Dataset using Pandas
          │
          ▼
Data Cleaning
• Handle Missing Values
• Clean Review Text
• Convert Text to Lowercase
• Remove Special Characters
          │
          ▼
Rule-Based Filtering
(Filter Reviews with Rating ≤ 2)
          │
          ▼
Keyword Frequency Analysis
(Collections.Counter)
          │
          ▼
Top 3 Complaint Keywords
          │
          ▼
Select 3 Critical Reviews
          │
          ▼
Generate Personalized Apology Emails
using Google Gemini API
```

---

# Data Cleaning Approach

The following preprocessing steps were performed before analysis:

* Loaded the dataset using Pandas.
* Inspected dataset dimensions and structure.
* Checked for missing values.
* Removed missing records where necessary.
* Standardized review text by converting it to lowercase.
* Removed unnecessary special characters and extra spaces.
* Prepared clean text for keyword analysis and AI processing.

---

# Rule-Based Filtering Logic

Instead of using Machine Learning, a rule-based approach was implemented.

The logic includes:

* Reviews with a rating of **1 or 2 stars** were classified as **Critical Reviews**.
* A predefined list of complaint keywords was created.
* Each critical review was searched for these keywords.
* Python string operations and **collections.Counter** were used to count keyword occurrences.
* The three most frequent complaint keywords were identified.

---

# Automated AI Response Generation

Three detailed critical customer reviews were selected from the filtered dataset.

Each review was sent to the Google Gemini API with a prompt instructing the model to act as a professional Customer Support Agent.

The AI generated:

* Personalized apology emails
* Empathetic responses
* Complaint-specific acknowledgements
* Professional customer support communication

---

# Output

The notebook produces the following outputs:

* Cleaned customer review dataset
* Filtered critical reviews
* Top complaint keywords
* Three AI-generated apology emails

---

# Installation

Install the required Python libraries before running the notebook.

```
pip install pandas google-generativeai
```

---

# API Key Setup

To generate AI responses, create a Google Gemini API key and configure it in the notebook.

Replace:

```python
genai.configure(api_key="YOUR_API_KEY")
```

with your own Gemini API key.

---

# How to Run the Project

1. Download the project files.
2. Install the required Python libraries.
3. Add your Google Gemini API key.
4. Open the Jupyter Notebook.
5. Run all notebook cells sequentially.
6. View the generated complaint analysis and AI response emails.

---

# Project Structure

```
Customer_Feedback_Analysis/

│── Customer_Feedback_Analysis.ipynb
│── Mobile Reviews Sentiment.csv
│── README.txt
```

---

# Skills Demonstrated

* Python Programming
* Data Cleaning
* Data Wrangling
* Text Processing
* Rule-Based Logic
* Keyword Frequency Analysis
* Prompt Engineering
* Google Gemini API Integration
* Customer Feedback Analysis
* Business Problem Solving

---

# Conclusion

This project demonstrates how Python and Generative AI can be combined to automate customer feedback analysis and improve customer support efficiency. By identifying critical reviews through rule-based filtering and generating personalized AI-powered apology emails, the solution reduces manual effort while providing consistent and empathetic responses. The project showcases practical skills in data preprocessing, text analysis, API integration, and business-oriented problem solving.


Author: Nitin Prasad
