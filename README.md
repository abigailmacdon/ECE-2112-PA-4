# ECE-2112-PA-4
**Made by: Abigail T. Macdon | 2ECE-B**

This repository contains the content of the *Programming Assignment 2* for the course subject **"Advanced Computer Programming and Algorithms"** for the First Semester of A.Y. 2026-2027

It includes three Python problems based on **Module 3 - Pandas** which are the following:

  **A. VISAYAS COMMUNICATION DATAFRAME**
 
  **B. VISAYAS FEMALE DATAFRAME**

  **C. CATEGORY-AVERAGE VISUALIZATION**

  Using the given CSV file named "cars" to load and create a DataFrame. Here is the link for the "cars.csv": https://github.com/abigailmacdon/ECE-2112-PA-3/blob/main/cars.csv.

To load the file this code is needed:

```python
import pandas as pd

df = pd.read_csv('board2.csv') 
df
```

• `import pandas as pd` - This imports the Pandas library and uses "pd" as a shorter term when coding.

• `pd.read_csv()` - reads the csv files uploaded to make it the DataFrame.

**Required DataFrame:**

• `Average` - in order to complete the required columns from the dataset. Make another DataFrame code to calculate the mean of Math, Electronics, GEAS and Communication

• New DataFrame with Average Column: To assign or insert the new Average column, this code was utilized:

                                 `python
                                  df = df.assign(Average=Average)
                                  df
                                  `
                                  
# **A. VISAYAS COMMUNICATION DATAFRAME**
Create a DataFrame named VisComm containing students whose Hometown is Visayas and whose Track
is Communication. Retain only these columns, in the stated order:

```python
                                        Name, Gender, Math, Electronics, Average
```

# **B. VISAYAS FEMALE DATAFRAME**
Create a second DataFrame named VisFemale containing students whose Hometown is Visayas and
whose Gender is Female. Retain only:

```python
                                        Name, Track, GEAS, Electronics, Average
```

# **C. CATEGORY-AVERAGE VISUALIZATION**

   ***c.1. For each feature, compute the mean of Average for every category using Pandas.***

   
   ***c.2. Display the three summary tables.***

   
   ***c.3. Create one figure containing three bar charts: mean Average by Track, by Gender, and by
Hometown.***


   ***c.4. Below the figure, write three concise statements identifying the category with the highest sample mean for each feature.***

   


***Thank you for reading!***

To see the detailed and main python program for Program Assignment 3, please click this link: **https://github.com/abigailmacdon/ECE-2112-PA-3/blob/main/Programming_Assignment_3.ipynb** and download. Open on Jupyter Notebook or Colab Notebooks, then run all the cells.

**README file Version History:**

September 16, 2026
  - Initial README draft.
