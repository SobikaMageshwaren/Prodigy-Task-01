🎨 Data Visualization using Matplotlib and Seaborn

This project demonstrates how to create simple yet effective data visualizations using Matplotlib and Seaborn in Python. The task involves generating two types of plots: a bar chart to display the gender distribution and a histogram to represent the age distribution in the dataset.

📋 Prerequisites
Before running the project, ensure you have the following Python libraries installed:

Matplotlib
Seaborn
Pandas
If these libraries are not installed, you can quickly install them using pip:

pip install matplotlib seaborn pandas

📊 Data
The sample data used in this project is a small dataset consisting of gender and age information for 10 individuals. The data is structured as follows:


data = {
    'Gender': ['Male', 'Female', 'Male', 'Female', 'Male', 'Female', 'Male', 'Female', 'Male', 'Female'],
    'Age': [23, 45, 31, 25, 34, 40, 28, 37, 29, 33]
}

📈 Visualizations
1. Gender Distribution
A bar chart is created to display the distribution of genders in the dataset. The chart provides a quick overview of the number of males and females in the sample.

Code:
plt.figure(figsize=(8, 6))
sns.countplot(x='Gender', data=df, palette='viridis')
plt.title('Gender Distribution')
plt.xlabel('Gender')
plt.ylabel('Count')
plt.show()

Output:
![Screenshot (179)](https://github.com/user-attachments/assets/2b51d7ee-a6fb-4f67-831a-271532cf82b4)


2. Age Distribution
A histogram is used to represent the age distribution of the individuals in the dataset. The histogram includes a Kernel Density Estimate (KDE) to show the probability density function of the ages.

Code:

plt.figure(figsize=(8, 6))
sns.histplot(df['Age'], bins=5, kde=True, color='blue')
plt.title('Age Distribution')
plt.xlabel('Age')
plt.ylabel('Frequency')
plt.show()
Output:
![Screenshot (180)](https://github.com/user-attachments/assets/7e58b34d-2068-4125-8270-fa9cca71072c)


🚀 Usage
To run this project, simply execute the Python script containing the code provided above. The script will generate the bar chart and histogram in separate windows.

python data_visualization.py

💡 Insights
These visualizations provide useful insights into the dataset:
Gender Distribution: A clear visual representation of the balance between males and females.
Age Distribution: A breakdown of the age range in the dataset, with additional insight into the density and concentration of ages through the KDE.

🔧 Tech Stack
Python
Matplotlib
Seaborn
Pandas

🎯 Conclusion
This project highlights the power of data visualization in making datasets more comprehensible and actionable. With just a few lines of code, Matplotlib and Seaborn help uncover patterns and trends that are otherwise hard to spot.
