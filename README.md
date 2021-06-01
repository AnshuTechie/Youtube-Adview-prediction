# Youtube-Adview-prediction
This project aims to build a Machine Learning Regression to predict Youtube adview counnt based on other youtube matrics.  

import pandas as pd;
df=pd.read_csv('advertising.csv')

df.head()
df.tail()

df.info()
df.describe()

df.drop('Ad Topic line',axis=1,inplace=True)
df.drop('City',axis=1,inplace=True)
df.drop('Country',axis=1,inplace=True)
df.drop('Timestamp',axis=1,inplace=True)

df.head()
y=df['clicked on Ad']
df.drop('clicked on Ad',axis=1,inplace=True)
x=df

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2)

from sklearn.linear_model import LogisticRegression
lm=LogisticRegression()
lm.fit(x_train,y_train)

lm.score(x_test,y_test)

df.hist(figsize=(10,11))
plt.show()

