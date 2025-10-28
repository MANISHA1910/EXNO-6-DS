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

# Coding and Output:
 
 ```
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
df=pd.read_csv("titanic_dataset.csv")
df.head()
```

## OUTPUT 
<img width="1793" height="518" alt="image" src="https://github.com/user-attachments/assets/e178d6e6-0259-4a05-9b1e-d7c8fb71456c" />

# 1. LINE PLOT

```
x=[1,2,3,4,5]
y=[3,6,2,7,1]
sns.lineplot(x=x,y=y)
plt.title('Line Plot')
```


## OUTPUT
<img width="1599" height="788" alt="image" src="https://github.com/user-attachments/assets/d901d7be-d7c8-4435-a1c3-6e0fc3c0d80e" />




# 2. MULTILINE PLOT
```
x=[1,2,3,4,5]
y1=[3,5,2,6,1]
y2=[1,6,4,3,8]
y3=[5,2,7,1,4]
sns.lineplot(x=x,y=y1)
sns.lineplot(x=x,y=y2)
sns.lineplot(x=x,y=y3)
plt.title('Multi Line Plot')
```


## OUTPUT
<img width="1114" height="658" alt="image" src="https://github.com/user-attachments/assets/d5ad525c-9ac8-47d7-b470-6c1c49920059" />



# TO VISUALIZE RELATIONSHIPS




# 1. BAR CHART
```
plt.figure(figsize=(8,5))
sns.barplot(x='Embarked',y='Fare',data=df,palette='rainbow')
plt.title("Fare Of Passenger By Embarked Town")
```


## OUTPUT
<img width="983" height="694" alt="image" src="https://github.com/user-attachments/assets/d0d09ef3-350f-4f28-b191-b35ec7b44932" />

# 2.SCATTER PLOT
```
sns.scatterplot(x="Age", y="Fare", data=df)
plt.title('Scatterplot of Age vs Fare')
plt.show()
```


## OUTPUT
<img width="1094" height="587" alt="image" src="https://github.com/user-attachments/assets/ca2d47e4-1854-47f3-b110-b77f564b829a" />


# 3.BUBBLE CHART
```
sns.scatterplot(x="Age", y="Fare", size="Pclass", data=df, sizes=(30, 200))
plt.title('Bubble Chart of Age vs Fare, Size by Passenger Class')
plt.show()
```

## OUTPUT
<img width="1003" height="576" alt="image" src="https://github.com/user-attachments/assets/05856258-36e4-4c5b-b11d-5317bc161721" />

# TO CAPTURE DISTRIBUTIONS
# 1. HISTOGRAM

```
sns.histplot(data=df,x="Pclass",hue="Survived",kde=True)
```


## OUTPUT
<img width="1159" height="536" alt="image" src="https://github.com/user-attachments/assets/5f9452e7-e5a7-4fe7-87b0-f711778c4c10" />


# 2.BOX PLOT

```
sns.boxplot(x='Pclass',y='Age',data=df,palette='rainbow')
plt.title("Age By Passenger Class")
```

## OUTPUT
<img width="931" height="665" alt="image" src="https://github.com/user-attachments/assets/ec26b07e-a4aa-4b23-af7a-215b95213eba" />


# 3. VIOLIN PLOT 

```
sns.violinplot(x="Pclass", y="Fare", data=df)
plt.title('Violin Plot of Fare by Passenger Class')
plt.show()
```

## OUTPUT
<img width="1050" height="594" alt="image" src="https://github.com/user-attachments/assets/0c6d17b3-d714-4578-ad58-a683b7eb13ca" />


# 4. DENSITY PLOT
```
sns.kdeplot(data=df['Age'], shade=True)
plt.title('Density Plot of Passenger Ages')
plt.show()
```

## 4.OUTPUT

<img width="1015" height="685" alt="image" src="https://github.com/user-attachments/assets/cf3135b4-986e-42db-b7eb-3f23dd4e4693" />


# 5. HEAT MAP
```
numeric_df = df.select_dtypes(include=['float64', 'int64'])
corr_matrix = numeric_df.corr()
sns.heatmap(corr_matrix, annot=True, cmap='coolwarm')
plt.title('Heatmap of Titanic Dataset')
plt.show()
```

## OUTPUT
<img width="1122" height="657" alt="image" src="https://github.com/user-attachments/assets/8c1a85ef-95ea-4a56-b978-d0a477eb797d" />












# Result:
Thus, the Data Visualization using seaborn python library for the given data is implemented successfully
