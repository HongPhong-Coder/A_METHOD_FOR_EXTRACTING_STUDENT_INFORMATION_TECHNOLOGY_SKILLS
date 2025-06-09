# IT Skill Gap Analysis using Machine Learning

## Overview

This project focuses on extracting and identifying the missing Information Technology (IT) skills of students from the Faculty of Information Technology at Van Lang University. It leverages machine learning models to classify and analyze student and company data, aiming to pinpoint skill gaps and relevant keywords.

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

* **Timeframe:** 09/2024 - 01/2025
* **Team Size:** 1 (Individual Research Project)

## Technology Stack

This project is built using the following technologies:

* **Language:** Python
* **Libraries:**
    * [pandas](https://pandas.pydata.org/) (Data manipulation and analysis)
    * [numpy](https://numpy.org/) (Numerical operations)
    * [matplotlib](https://matplotlib.org/) (Data visualization)
    * [nltk](https://www.nltk.org/) (Natural Language Toolkit)
    * [yake](https://github.com/LIAAD/yake) (Yet Another Keyword Extractor)
    * [scikit-learn (sklearn)](https://scikit-learn.org/stable/) (Machine Learning models and utilities)
    * [gensim](https://radimrehurek.com/gensim/) (Topic modeling and similarity analysis)

## Getting Started

Follow these steps to set up and run the project:

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/HongPhong-Coder/A-METHOD-FOR-EXTRACTING-STUDENT-INFORMATION-TECHNOLOGY-SKILLS.git](https://github.com/HongPhong-Coder/A-METHOD-FOR-EXTRACTING-STUDENT-INFORMATION-TECHNOLOGY-SKILLS.git)
    cd A-METHOD-FOR-EXTRACTING-STUDENT-INFORMATION-TECHNOLOGY-SKILLS
    ```

2.  **Install Dependencies:**
    It is highly recommended to create a virtual environment before installing dependencies.
    ```bash
    pip install -r requirements.txt
    ```
    *(You will need to create a `requirements.txt` file in the root directory of your project, listing all the libraries from the "Technology Stack" section. Example content for `requirements.txt`:)*
    ```
    pandas
    numpy
    matplotlib
    nltk
    yake
    scikit-learn
    gensim
    ```

3.  **Data Acquisition and Preparation:**
    * Ensure all necessary raw student data files are placed within the `Data/` directory.
    * To acquire the `company_data`, run the `Get_Data.py` script. This script is designed to scrape data from CareerViet.vn and will typically save the processed data into the `Data/` directory.
        ```bash
        python Get_Data.py
        ```
    * *(Optional)* If you wish to check data freshness or potential duplicates, you can run `Get_More_Data.py`.
        ```bash
        python Get_More_Data.py
        ```
    * After running the necessary data acquisition scripts and placing all data, ensure that all required datasets (student data and company data) are correctly located in the `Data/` directory for the main analysis.

4.  **Run the Analysis:**
    * Open the `Classification_Algorithm.ipynb` notebook using a Jupyter environment (such as VS Code with Jupyter extension, Google Colab, or a local Jupyter Notebook server).
    * Execute the cells sequentially within the notebook. The `Classification_Algorithm.ipynb` notebook is designed to handle all subsequent steps, including loading data from the `Data/` folder, performing data processing, training machine learning models, and executing the skill extraction process.

## Project Structure

.
├── .idea/                     # Cấu hình cụ thể cho IDE (ví dụ: cài đặt PyCharm)
├── .ipynb_checkpoints/        # Các điểm lưu (checkpoint) của Jupyter notebook
├── Data/                      # Thư mục chứa tất cả các tập dữ liệu (dữ liệu thô và đã xử lý)
├── Classification_Algorithm.ipynb # Notebook chính cho việc phân loại và phân tích ML
├── Get_Data.py                # Script để cào dữ liệu công ty từ CareerViet.vn và lưu vào thư mục Data/
├── Get_More_Data.py           # Script để kiểm tra độ mới của dữ liệu và khả năng trùng lặp dựa trên thời gian chỉnh sửa
├── pyenv.cfg                  # Cấu hình môi trường Python
├── .gitignore                 # Chỉ định các tệp không cần theo dõi để bỏ qua một cách có chủ đích
├── LICENSE                    # Giấy phép của dự án
└── README.md                  # Tệp README này

## Results & Visualizations (Optional - *Add actual screenshots/charts here*)

* **Model Performance:** Metrics (e.g., accuracy, precision, recall) for each machine learning model used.
* **Skill Gap Analysis:** Visualizations highlighting discrepancies between student skills and industry requirements.
* **Extracted Keywords:** Examples of keywords extracted by YAKE for different IT majors.

## Contact

For any inquiries or further information, please contact:
* **HongPhong-Coder** - lehongphong061203@gmail.com

---
