# ECE-2112-PA-4
**Made by: Abigail T. Macdon | 2ECE-B**

This repository contains the content of the *Programming Assignment 4* for the course subject **"Advanced Computer Programming and Algorithms"** for the First Semester of A.Y. 2026-2027

It includes three Python problems based on **Module 4 - Data Wrangling and Visualization** which are the following:

  **A. VISAYAS COMMUNICATION DATAFRAME**
 
  **B. VISAYAS FEMALE DATAFRAME**

  **C. CATEGORY-AVERAGE VISUALIZATION**

  Using the given XLSX file named "board2", I converted the file into a CSV file to load and create a DataFrame. Here is the link for the "board2.csv": https://github.com/abigailmacdon/ECE-2112-PA-4/blob/main/board2.csv.

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

• **New DataFrame with Average Column**: To assign or insert the new Average column, this code was utilized:

 ```python
 df = df.assign(Average=Average)
 df
 ```
                                  
# **A. VISAYAS COMMUNICATION DATAFRAME**
Create a DataFrame named VisComm containing students whose Hometown is Visayas and whose Track
is Communication. Retain only these columns, in the stated order:

```python
                                        Name, Gender, Math, Electronics, Average
```

• `Hometown == Visayas` - In order to only filter or show the data from students whose Hometown is Visayas.

• `Track == Communication` - Set in order to show students that studies the Communication Track.

• `&` - Used to combine the two filtering conditions.

• `Name` - Shows the name in the first column of the students that Hometown is in Visayas and has a Track in Communication.

• `Gender` - Shows the gender in the second column of the students that Hometown is in Visayas and has a Track in Communication.

• `Math` - Shows the Math in the third column of the students that Hometown is in Visayas and has a Track in Communication.

• `Electronics` - Shows the Electronics in the fourth column of the students that Hometown is in Visayas and has a Track in Communication.

• `Average` - Shows the Average in the fifth column of the students that Hometown is in Visayas and has a Track in Communication.


# **B. VISAYAS FEMALE DATAFRAME**
Create a second DataFrame named VisFemale containing students whose Hometown is Visayas and
whose Gender is Female. Retain only:

```python
                                        Name, Track, GEAS, Electronics, Average
```

• `Hometown == Visayas` - In order to only filter or show the data from students whose Hometown is Visayas.

• `Gender == Female` - Set in order to show students that gender is Female.

• `&` - Used to combine the two filtering conditions.

• `Name` - Shows the name in the first column of the students that Hometown is in Visayas and is a female.

• `Track` - Shows the track in the second column of the students that Hometown is in Visayas and is a female.

• `GEAS` - Shows the GEAS in the third column of the students that Hometown is in Visayas and is a female.

• `Electronics` - Shows the Electronics in the fourth column of the students that Hometown is in Visayas and is a female.

• `Average` - Shows the Average in the fifth column of the students that Hometown is in Visayas and is a female.


# **C. CATEGORY-AVERAGE VISUALIZATION**

   ***c.1. For each feature, compute the mean of Average for every category using Pandas.***

• `Communication` - Stores the mean Average of students under the Communication Track.

• `Instrumentation` - Stores the mean Average of students under the Instrumentation Track.

• `Microelectronics` - Stores the mean Average of students under the Microelectronics Track.4

• `Female` - Stores the mean Average of female students.

• `Male` - Stores the mean Average of male students.

• `Luzon` - Stores the mean Average of students from Luzon.

• `Visayas` - Stores the mean Average of students from Visayas.

• `Mindanao` - Stores the mean Average of students from Mindanao.

• `.mean()` - Calculates the mean or average of the selected values.
   
   ***c.2. Display the three summary tables.***
   
• `TrackMean` - Stores the mean Average for each Track category.

• `GenderMean` - Stores the mean Average for each Gender category.

• `HometownMean` - Stores the mean Average for each Hometown category.
   
   ***c.3. Create one figure containing three bar charts: mean Average by Track, by Gender, and by
Hometown.***

• `import matplotlib.pyplot as plt` - Imports Matplotlib and uses plt as a shorter term for coding.

• `plt.subplots()` - Creates one figure with three graphs.

• `plot(kind='bar')` - Creates a bar graph using the summary tables.

• `set_title()` - Adds the title of each graph.

• `set_xlabel()` - Adds the label for the x-axis.

• `set_ylabel()` - Adds the label for the y-axis.

• `plt.tight_layout()` - Adjusts the spacing between the graphs.

• `plt.show()` - Displays the completed figure.

   ***c.4. Below the figure, write three concise statements identifying the category with the highest sample mean for each feature.***

• `.idxmax()` - Finds the position of the highest value.

• `.loc[]` - Gets the category from the row containing the highest mean Average.

Based on the calculated sample means:

```python
Communication has the highest sample mean Average garnering 67.975 among the Track categories.
Male has the highest sample mean Average amounting to 65.225 among the Gender categories.
Luzon has the highest sample mean Average of 67.500 among the Hometown categories
```
   


***Thank you for reading!***

To see the detailed and main python program for Program Assignment 4, please click this link: **https://github.com/abigailmacdon/ECE-2112-PA-4/blob/main/Programming_Assignment_4.ipynb** and download. Open on Jupyter Notebook or Colab Notebooks, then run all the cells.

**README file Version History:**

September 16, 2026
  - Initial README draft.
