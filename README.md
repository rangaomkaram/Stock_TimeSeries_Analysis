# Stock_TimeSeries_Analysis
Analysis Of Share price of Tesla and Microsoft

##Tesla High stock units from year 2017 - 2022
![image](https://user-images.githubusercontent.com/46269446/159546874-ee3876fb-c9cf-49ed-bb40-8d1850e901d7.png)

##Time Sampling of the TESLA data of Rule A (Year End Frequency)
![image](https://user-images.githubusercontent.com/46269446/159547207-569b8cb7-e837-42f4-bb33-6544663bb02a.png)

#Time Resamping rules
#Rule :
"""
rule = A , year end frequency
rule = QS, quartely frequency
rule = BA ,Business End Frequency
rule = BQS Business Quarters
"""

```
df_Tesla.resample(rule = 'BA').max().plot(kind='bar')
```
![image](https://user-images.githubusercontent.com/46269446/159547623-40faa74d-50a5-4ac5-9dab-e4ea785365f9.png)
```
df_Tesla['Open'].resample(rule = 'BA').max().plot(kind = 'bar')
```
![image](https://user-images.githubusercontent.com/46269446/159547705-7c973640-625c-4316-aa33-16198401408e.png)
```
Tesla['Open'].resample(rule = 'BA').mean().plot(kind = 'bar')
```

![image](https://user-images.githubusercontent.com/46269446/159547790-0038059f-440d-42d1-a2b3-4fbbd31ee8d8.png)
```
df_Tesla['Open'].resample(rule = 'A').mean().plot(kind='bar')
```

![image](https://user-images.githubusercontent.com/46269446/159547867-3f6b01c7-1c9f-476b-ac69-3dbabb25c646.png)
```
df_Tesla[['Open','Open:30 days rolling']].plot(figsize=(12,6))
```

![image](https://user-images.githubusercontent.com/46269446/159548016-3c6e4453-9205-45c4-a4e9-e5deab8e7e87.png)



