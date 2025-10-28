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
# OUTPUT
<img width="1793" height="518" alt="506491975-e178d6e6-0259-4a05-9b1e-d7c8fb71456c" src="https://github.com/user-attachments/assets/c1d35d8a-8092-4b36-9bd8-eef5529d1890" />

# 1.LINE PLOT


```
x=[1,2,3,4,5]
y=[3,6,2,7,1]
sns.lineplot(x=x,y=y)
plt.title('Line Plot')
```

# OUTPUT


<img width="1599" height="788" alt="506492356-d901d7be-d7c8-4435-a1c3-6e0fc3c0d80e" src="https://github.com/user-attachments/assets/71b884df-f8e5-4347-b5bd-b4c165c821b2" />

# 2.MULTILINE PLOT

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

# OUTPUT
<img width="1114" height="658" alt="506492817-d5ad525c-9ac8-47d7-b470-6c1c49920059" src="https://github.com/user-attachments/assets/8757ea9e-f3f9-4094-ad09-1df833710ec9" />


# TO VISUALIZE RELATIONSHIPS
# 1. BAR CHARTS


```
plt.figure(figsize=(8,5))
sns.barplot(x='Embarked',y='Fare',data=df,palette='rainbow')
plt.title("Fare Of Passenger By Embarked Town")
```

# OUTPUT
<img width="983" height="694" alt="506493155-d0d09ef3-350f-4f28-b191-b35ec7b44932" src="https://github.com/user-attachments/assets/e384d206-2b76-4379-b079-8688ddaec43a" />

2. SCATTER PLOT


```
   sns.scatterplot(x="Age", y="Fare", data=df)
   plt.title('Scatterplot of Age vs Fare')
   plt.show()
```

# OUTPUT

   <img width="1094" height="587" alt="506493522-ca2d47e4-1854-47f3-b110-b77f564b829a" src="https://github.com/user-attachments/assets/0b1c0e00-9a51-4bdb-b894-db64deb847af" />

# 3.BUBBLE CHART

```
sns.scatterplot(x="Age", y="Fare", size="Pclass", data=df, sizes=(30, 200))
plt.title('Bubble Chart of Age vs Fare, Size by Passenger Class')
plt.show()
```
# OUTPUT

<img width="1003" height="576" alt="506493853-05856258-36e4-4c5b-b11d-5317bc161721" src="https://github.com/user-attachments/assets/f121f7f9-a720-496a-99de-7bedc68c3b3b" />

# TO CAPTURE DISTRIBUTIONS

# 1.HISTOGRAM

```
sns.histplot(data=df,x="Pclass",hue="Survived",kde=True)
```

# OUTPUT
<img width="1159" height="536" alt="506494161-5f9452e7-e5a7-4fe7-87b0-f711778c4c10" src="https://github.com/user-attachments/assets/3483dd52-71a4-45ea-ab4a-76bcbaf0f9bd" />


# 2.BOX PLOT

```
sns.boxplot(x='Pclass',y='Age',data=df,palette='rainbow')
plt.title("Age By Passenger Class")

```

# OUTPUT

<img width="931" height="665" alt="506494390-ec26b07e-a4aa-4b23-af7a-215b95213eba" src="https://github.com/user-attachments/assets/3d6fc03a-6520-411c-8b04-baba4cf8d529" />

# 3.VIOLIN PLOT  

```
sns.violinplot(x="Pclass", y="Fare", data=df)
plt.title('Violin Plot of Fare by Passenger Class')
plt.show()

```

# OUTPUT 


<img width="1050" height="594" alt="506494771-0c6d17b3-d714-4578-ad58-a683b7eb13ca" src="https://github.com/user-attachments/assets/97a9f5a5-932f-42cc-82c1-16e944f7735a" />


# 4.DENSITY PLOT

```
sns.kdeplot(data=df['Age'], shade=True)
plt.title('Density Plot of Passenger Ages')
plt.show()

```

# OUTPUT
<img width="1015" height="685" alt="506495131-cf3135b4-986e-42db-b7eb-3f23dd4e4693" src="https://github.com/user-attachments/assets/0fd44c2c-ca2a-4dcc-be6d-0f2fd0398bd8" />


# 5. HEAT MAP

```
sns.kdeplot(data=df['Age'], shade=True)
plt.title('Density Plot of Passenger Ages')
plt.show()
```

# OUTPUT

<img width="1122" height="657" alt="506495614-8c1a85ef-95ea-4a56-b978-d0a477eb797d" src="https://github.com/user-attachments/assets/54bb7fd9-3e71-40fc-8079-f258c8959517" />







# Result:
 Include your result here
