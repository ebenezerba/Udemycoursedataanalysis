# Udemy Dataset Analysis
Welcome to UdemyCourseAnalysis, a repository dedicated to the in-depth examination of a comprehensive dataset of Udemy courses. Our primary objective is to unveil valuable insights and discern trends within the expansive landscape of online learning offered on Udemy, leveraging the power of Python for data analysis.




## Introduction
This project involves loading a dataset from Udemy, exploring the data, and visualizing the distribution of course ratings using Python libraries such as Pandas, Matplotlib, and Seaborn.

## Steps

1. Import the necessary libraries:
    ```python
    import pandas as pd
    import matplotlib.pyplot as plt
    import seaborn as sns
    ```


2. Load the dataset:
    ```python
    udemy = pd.read_csv("/content/udemy.csv")
    ```


3. Display the first 300 rows of the dataset:
    ```python
    udemy.head(300)
    ```


4. Explore unique values in each column:
    ```python
    for col in udemy.columns:
        print(f"Unique values in column '{col}':")
        print(udemy[col].unique())
        print()
    ```


5. Generate descriptive statistics of the dataset:
    ```python
    udemy.describe()
    ```


6. Set the style of Seaborn:
    ```python
    sns.set(style="whitegrid")
    ```


7. Visualize the distribution of course ratings:
    ```python
    plt.figure(figsize=(10, 6))
    sns.histplot(udemy['avg_rating'], bins=30, kde=True, color='skyblue')
    plt.title('Distribution of Course Ratings on Udemy')
    plt.xlabel('Average Rating')
    plt.ylabel('Frequency')
    plt.show()
    ```

## Conclusion
This README file provides an overview of loading the Udemy dataset, exploring its contents, and visualizing the distribution of course ratings using Python data analysis libraries.

## Reference
1.Kaggle


## Contact
Ebenezer Boako-Aggrey - @www.linkedin.com/in/eboakoaggrey - eboako@mail.com

Project Link: https://github.com/your_username/repo_name
