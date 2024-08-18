Data Visualization using Matplotlib and Seaborn
This project demonstrates how to create simple data visualizations using Matplotlib and Seaborn in Python. The task involves generating two types of plots: 
a bar chart to display the gender distribution and a histogram to represent the age distribution in the dataset.

Prerequisites
Ensure you have the following Python libraries installed:
matplotlib
seaborn
pandas
You can install these using pip if they are not already installed:

pip install matplotlib seaborn pandas
Data
The sample data used in this project is a small dataset consisting of gender and age information for 10 individuals. The data is structured as follows:

data = {
    'Gender': ['Male', 'Female', 'Male', 'Female', 'Male', 'Female', 'Male', 'Female', 'Male', 'Female'],
    'Age': [23, 45, 31, 25, 34, 40, 28, 37, 29, 33]
}

Visualizations
1. Gender Distribution
A bar chart is created to display the distribution of genders in the dataset. The chart provides a quick overview of the number of males and females in the sample.


Code
plt.figure(figsize=(8, 6))
sns.countplot(x='Gender', data=df, palette='viridis')
plt.title('Gender Distribution')
plt.xlabel('Gender')
plt.ylabel('Count')
plt.show()

2. Age Distribution
A histogram is used to represent the age distribution of the individuals in the dataset. The histogram includes a kernel density estimate (KDE) to show the probability density function of the ages.

Code:
plt.figure(figsize=(8, 6))
sns.histplot(df['Age'], bins=5, kde=True, color='blue')
plt.title('Age Distribution')
plt.xlabel('Age')
plt.ylabel('Frequency')
plt.show()

Usage
To run this project, simply execute the Python script containing the code provided above. The script will generate the bar chart and histogram in separate windows.
