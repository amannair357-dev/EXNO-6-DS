# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY

# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding:

```
import seaborn as sns
import matplotlib.pyplot as plt
df=sns.load_dataset("iris")
df.head()
corr_matrix=df.select_dtypes(include=["float64"]).corr()
sns.heatmap(corr_matrix, annot=True, cmap="coolwarm")
plt.show()
sns.jointplot(x='sepal_length',y='sepal_width',data=df,kind='hex')
sns.jointplot(x='sepal_length',y='sepal_width',data=df,kind='reg')
sns.pairplot(df)
sns.pairplot(df,hue='species')
sns.distplot(df['sepal_width'])
sns.distplot(df['petal_length'],kde=False,bins=10)
sns.countplot(x='species',data=df)
sns.countplot(y='species',data=df)
sns.barplot(x='sepal_length',y='sepal_width',data=df)
sns.boxplot(x='sepal_length',y='sepal_width',data=df)
sns.boxplot(x='sepal_length',y='sepal_width',data=df,palette='rainbow')
sns.boxplot(data=df,orient='v')sns.boxplot(x='sepal_length',y='sepal_width',data=df,hue='species')
sns.violinplot(x='sepal_length',y='sepal_width',data=df,palette='rainbow')

```
# Output:

![alt text](<Screenshot 2026-03-16 220419-1.png>) 
![alt text](<Screenshot 2026-03-16 220429-1.png>)
![alt text](<Screenshot 2026-03-16 220437-1.png>) 
![alt text](<Screenshot 2026-03-16 220451-1.png>) 
![alt text](<Screenshot 2026-03-16 220503-1.png>) 
![alt text](<Screenshot 2026-03-16 220511-1.png>) 
![alt text](<Screenshot 2026-03-16 220519-1.png>) 
![alt text](<Screenshot 2026-03-16 220526-1.png>) 
![alt text](<Screenshot 2026-03-16 220533-1.png>) 
![alt text](<Screenshot 2026-03-16 220540-1.png>) 
![alt text](<Screenshot 2026-03-16 220548-1.png>) 
![alt text](<Screenshot 2026-03-16 220555-1.png>) 
![alt text](<Screenshot 2026-03-16 220602-1.png>)
![alt text](<Screenshot 2026-03-16 220610-1.png>) 
![alt text](<Screenshot 2026-03-16 220615-1.png>) 
![alt text](<Screenshot 2026-03-16 220402-1.png>)

# Result:

Thus,The data visualization using seaborn library is completed successfully
