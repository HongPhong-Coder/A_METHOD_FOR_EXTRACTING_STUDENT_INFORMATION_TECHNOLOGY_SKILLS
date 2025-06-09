# IT Skill Extraction using Machine Learning

## Overview

This project focuses on extracting the missing Information Technology (IT) skills of students from the Faculty of Information Technology at Van Lang University. It leverages machine learning models to classify and analyze learning data, ultimately identifying skill gaps.

## Project Details

* **Objective:** To extract missing IT skills from student and company data, employing various machine learning techniques and natural language processing for keyword extraction.
* **Data Sources:**
    * **Student Data:** Includes subjects from the training program and corresponding skills for each subject.
    * **Company Data:** Contains company names and the IT skills they typically hire for.
* **Methodology:**
    1.  **Data Processing & Cleaning:** Applying techniques to prepare both student and company datasets.
    2.  **Model Training & Optimization:** Utilizing GridSearchCV for parameter optimization to enhance accuracy across 5 machine learning models:
        * Support Vector Machine (SVM)
        * Decision Tree
        * K-Nearest Neighbors (KNN)
        * Random Forest
        * Logistic Regression
    3.  **Keyword Extraction:** Employing the YAKE (Yet Another Keyword Extractor) technique to extract relevant student keywords categorized by 4 main majors in the IT field.

* **Timeframe:** 09/2024 - 01/2025 (Individual research project)

## Technology Stack

This project is built using the following technologies:

* **Language:** Python
* **Libraries:**
    * [pandas](https://pandas.pydata.org/) (Data manipulation and analysis)
    * [numpy](https://numpy.org/) (Numerical operations)
    * [matplotlib](https://matplotlib.org/) (Data visualization)
    * [nltk](https://www.nltk.org/) (Natural Language Toolkit)
    * [yake](https://github.com/LIAAD/yake) (Yet Another Keyword Extractor)
    * [scikit-learn (sklearn)](https://scikit-learn.org/stable/) (Machine learning models and utilities)
    * [gensim](https://radimrehurek.com/gensim/) (Topic modeling and similarity analysis - potentially for keyword processing)

* **Team Size:** 1 (Individual Research Project)

## Getting Started

To get started with this project, follow these steps:

1.  **Clone the Repository:**
    ```bash
    !git clone [YOUR_REPOSITORY_URL_HERE]
    %cd [YOUR_REPOSITORY_NAME] # Navigate into the project directory (e.g., IT_Skill_Extraction_ML)
    ```
    *(Replace `[YOUR_REPOSITORY_URL_HERE]` with the actual URL of your GitHub repository. And `[YOUR_REPOSITORY_NAME]` with the actual name you set for your repository, e.g., `IT_Skill_Extraction_ML`)*

2.  **Install Dependencies:**
    It is highly recommended to create a virtual environment.
    ```bash
    pip install -r requirements.txt
    ```
    *(You will need to create a `requirements.txt` file listing all the libraries from the "Technology Stack" section. Example content for `requirements.txt`:)*
    ```
    pandas
    numpy
    matplotlib
    nltk
    yake
    scikit-learn
    gensim
    ```

3.  **Data Preparation:**
    * Ensure your `student_data` and `company_data` (or similar named datasets) are placed in the appropriate directory (e.g., a `data` folder).
    * [Link to your Dataset (optional)]: If your data is publicly available, provide a link here.

4.  **Run the Main Script/Notebook:**
    * Identify the main script or Jupyter Notebook (`.ipynb`) that orchestrates the data processing, model training, and skill extraction.
    * Execute this script/notebook to run the project.

## Project Structure (Example - *Adjust based on your actual structure*)
