# PYTHON-TASK-PROJECT

Below is a Python project that aims at performing thorough data cleaning and then visualizing using Seaborn or Matplotlib on an imported dataset named "project". 
In the Data Cleaning attention is on column names, data types, and an extraction of the year and year-month from the date column for easier visualization.
add the number of days from when the movie was released till today (i.e the day you're doing the visualization)

# DATA CLEANING

# THE SCREENSHOT BELOW SHOWS CODE TO initial capitalize the columns headers
![PYTHON Pro 1  initial capitalizing the columns headers](https://github.com/Tonyigba/PYTHON-TASK-PROJECT/assets/143624967/71a9e8cf-1f38-47f2-8052-09f4c7306405)

# SCREENSHOT BELOW SHOWS CODE Replacing country's abbreviation with the country Names
![PYTHON CODE Replacing countries abreviation with the countries Names](https://github.com/Tonyigba/PYTHON-TASK-PROJECT/assets/143624967/9355cdcb-988c-4de6-94d8-28af204a4d51)

# SCREENSHOT BELOW SHOWS CODE USING REPLACE TO REMOVE THE BRACKETS IN THE DATE IN THE 1ST INSTANCE
![PYTHON  USING REPLACE TO REMOVE THE BRAKETS IN THE DATE IN THE 1ST INSTANCE](https://github.com/Tonyigba/PYTHON-TASK-PROJECT/assets/143624967/5071628a-c345-44d9-9ea7-5d97c6a16988)

# SCREENSHOT BELOW SHOWS CODE EXTRACTING THE YEAR FROM THE DATE AND CREATING THE COLUMN AS THE YEAR
![PYTHON EXTRACTION THE YEAR FROM THE DATE AND CREATING THE COLUMN AS YEAR](https://github.com/Tonyigba/PYTHON-TASK-PROJECT/assets/143624967/106067cf-9e97-445f-bf47-618c8848ce1d)

# SCREENSHOT BELOW SHOWS CODE assigning date datatype to date column
![PYTHON Pro 2 assigning date datatype to date column](https://github.com/Tonyigba/PYTHON-TASK-PROJECT/assets/143624967/40fdb98a-0fde-453e-a741-466dc607f1c4)

# SCREENSHOT BELOW SHOWS CODE CALCULATING THE NUMBER OF DAYS SINCE MOVIE WAS LISTED UNTIL TODAY AND CREATING THE COLUMN AS ADDED DAYS
![PYTHON CALCULATING THE NUMBER OF DAYS SINCE MOVIE WAS LISTED UNTIL TODAY AND CREATING THE COLUMN AS ADDED DAYS](https://github.com/Tonyigba/PYTHON-TASK-PROJECT/assets/143624967/c528c4cb-9fec-42b5-88a4-6ac4805e044e)

# FINAL CLEANED PROJECT DATASET AND SAVING TO CSV
![PROJET CLEANED DATA NAMED PRODATA](https://github.com/Tonyigba/PYTHON-TASK-PROJECT/assets/143624967/3404cffe-39d3-40e1-b7a1-a75df629a245)




# Questions to answer with the dataset:

1: The most popular director.

prodata['Director'].value_counts()[1:]

Top_Director
Top_Director.index[0:5]
Top_Director.values[0:5]
plt.bar(Top_Director.index[0:5], Top_Director.values[0:5], 0.2)
plt.title('Distribution of top Director')
plt.show()
![BAR CHART SHOWING THE MOST POPULAR DIRECTOR PNG 1](https://github.com/Tonyigba/PYTHON-TASK-PROJECT/assets/143624967/434f63f7-d073-4f04-a771-06a664ba3f27)

![THE MOST POPULAR DIRECTOR IS TO COUNT THE DIRECTOR THAT HAS THE MOST MOVE](https://github.com/Tonyigba/PYTHON-TASK-PROJECT/assets/143624967/f590d50a-4491-4c9f-83dc-b292bb8c8ec3)


2: The countries that make the most and least movies (top 5 and bottom 5)
prodata['Country'].value_counts().head()
prodata['Country'].value_counts().tail()
![THE CODE BELOW SHOWS THE FIVE TOP COUNTRY AND FIVE LAST COUNTRY](https://github.com/Tonyigba/PYTHON-TASK-PROJECT/assets/143624967/786f427e-0f98-4aa5-a176-9a04e074f9ce)

3: Movie trends over the years

4: Most popular country-genre mix



5: Countries with the highest average movie duration.

prodata.groupby('Country')['Duration'].mean().round(0).sort_values(ascending =False)[0:9]

Top_avg
Top_avg.index[0:6]
Top_avg.values[0:6]
plt.bar(Top_avg.index[0:6], Top_avg.values[0:6], 0.5)
plt.title('Distribution of Country with Highest Movie Duration')
plt.show()

![Countries with highest average movie duration](https://github.com/Tonyigba/PYTHON-TASK-PROJECT/assets/143624967/1e3145d7-1d2c-4974-8478-6fbeff60036c)

![Countries with highest average movie duration 2](https://github.com/Tonyigba/PYTHON-TASK-PROJECT/assets/143624967/87288e5d-1ea5-4310-a004-503df8c1c41b)

![GRAPHIC REPRESENTATION OF COUNTRIES WITH HIGHEST MOVIE DURATION](https://github.com/Tonyigba/PYTHON-TASK-PROJECT/assets/143624967/5459a38f-d740-432b-abff-56c85391b058)




