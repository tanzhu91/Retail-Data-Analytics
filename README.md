# Retail-Data-Analytics

## The aim of this project is to answer a few key questions. Which departments are leading in sales, which are the leading stores in those departments? The relationship between promotional markdowns and holidays and how that affects sales. What is the future direction of sales for the best performing department and store and for a poorly performing one ?



First thing we notice is the high amount of sales around 26th of November and 30 and 23-24 th December. While November 26 th is an official holiday in the United States 23rd of December is not but it is Christmas time so the high amount of sales that week makes sense.

![newplot](https://github.com/user-attachments/assets/e5aa2d9d-d972-46d4-90e1-a72baa0ee1a4)

Here we can see which days are officially holidays in the data. The week before and after December 31 st, there is huge drop in sales despite it being a holiday , suggesting a pattern of avoiding purchases by customers around the new year.

![newplot](https://github.com/user-attachments/assets/cfec1d07-69b3-46c6-ae2b-22db56bd3d66)


In this figure we can see the sales across departments and all 3 years. We can already see that some departments make much bigger share of the sales like number 92 , 95 , 38 , 72 , 40 and 2.

![newplot](https://github.com/user-attachments/assets/84e6ebae-1530-418d-ba2b-74441c1ddd33)


Here those top departments are selected and shown.

![newplot](https://github.com/user-attachments/assets/7073199f-5782-41aa-8ba8-c02b00ba7d23)



There was some really bad performing departmens in the data. The suprising thing was there is even one with negative amount of sales. Something mysterious is happening in Department 47. Sales in the negative are not possible, recommendations are to check for fraud.

![newplot](https://github.com/user-attachments/assets/40f9279d-d689-4640-a00d-37b013e08181)


Here Weekly sales are plotted against type of stores and amount of sales based on holiday or not. We can see store type A has the most holiday sales of all three.

![newplot](https://github.com/user-attachments/assets/d74e29e3-5157-4309-a883-36a6cce93779)



I decided to plot the stores of the best performing department based on sales and the worst one. We can see that department 92 has best performing stores numbered as follows: 14,2,20,13,4 and so on. The size is not always the biggest but most of them are close to the biggest possible.

![newplot](https://github.com/user-attachments/assets/06380c5a-8280-4816-b98c-67305e308455)


Worst performers in department 47 are store number 35,1,10,45 and so on.

![newplot](https://github.com/user-attachments/assets/1d8e61da-1c5d-43fc-9f63-d88b9f3602aa)



Here correlation between size of stores and weekly sales shows clearly there is a positive relationship. The bigger the store the more sales in total. The model is with an R value of 71 % , so it is quite good.

![newplot](https://github.com/user-attachments/assets/d9fd3189-a5d0-42d4-bdc7-7efca57fea60)


In this graph we can see the dates when promotional markdowns were available. A lot of them have a rise right before holidays or at holiday times.


![newplot](https://github.com/user-attachments/assets/19c8f870-e533-4829-b6fd-f17e7f5dcf1d)

And here we can see the correlation between markdowns and holidays.

![newplot](https://github.com/user-attachments/assets/e6fd74c7-927e-4943-8475-d6efe3b1facd)

Since weekly sales data is available only until October 2012 and markdowns start from November 2011, we can see when plotted all together the effects Markdowns and Holidays are having on sales. Particularly around the period of 25 November 2011 , from December 9 to December 30 - 2011 and around February 10 , 2012 and April 6 , 2012. Suprisingly even though there is a huge Markdown2 around December 30, 2011 and after , sales are dropping and quite low in that period.


![newplot](https://github.com/user-attachments/assets/3af6299a-5be6-4538-a2fd-83b179905290)


Predictive modelling using Prophet shows that combined sales for all departments will continue at the same pace until February 2013 and beyond with the same spike and dip around holiday times at the end of 2012, which can be seen as the blue line in the figure. Yhat is the predicted value in this case.

![image](https://github.com/user-attachments/assets/e1a71c65-0208-410d-a113-0668425b7003)



| Date       | yhat        | yhat_lower      | yhat_upper      |
|------------|-------------|-----------------|-----------------|
| 2012-11-11 | 16986.88    | -11795.84       | 46915.47        |
| 2012-11-18 | 17674.34    | -10517.20       | 45376.71        |
| 2012-11-25 | 18140.01    | -8673.53        | 46848.08        |
| 2012-12-02 | 18986.76    | -11622.29       | 47263.41        |
| 2012-12-09 | 20436.81    | -9317.61        | 51806.84        |
| 2012-12-16 | 21647.42    | -7429.43        | 62023.63        |
| 2012-12-23 | 21269.47    | -8594.95        | 51343.91        |
| 2012-12-30 | 18846.35    | -11763.30       | 46431.90        |
| 2013-01-06 | 15552.68    | -14793.90       | 43276.53        |


The best performing department number 92 also shows similar trends around the winter holiday periods with a spike and even a slight overall increase over time in sales.

![image](https://github.com/user-attachments/assets/19151199-987b-4075-8d9b-22ea9558d683)

|Date        |yhat         |yhat_lower       |yhat_upper       |
|------------|-------------|-----------------|-----------------|
|2012-11-11  |91096.08392  |27556.602698     |155299.108173    |
|2012-11-18  |93491.58790  |26683.066200     |155331.313681    |
|2012-11-25  |92616.97255  |27624.603418     |156126.876549    |
|2012-12-02  |91296.73408  |25430.116999     |147471.574248    |
|2012-12-09  |92020.887835 |30472.697049     |152654.506457    |
|2012-12-16  |93727.76185  |31967.241653     |155221.349540    |
|2012-12-23  |93054.49571  |32574.361850     |157994.130737    |
|2012-12-30  |88642.92735  |25564.696585     |148292.776335    |
|2013-01-06  |83284.166012 |22881.500197     |149800.266710    |


However the best performing store number 14 from the same department is on a downward trend.

![image](https://github.com/user-attachments/assets/0a8dd1c5-d76b-4ba3-b5fc-b68d2b014e64)


One of the badly performing departments number 54 is also on a decline. Two spikes around holiday periods can be seen and the third one as a prediction. Recommendations would be to check the reason why ineffective departments are underperforming and also concentrate on boosting better performing ones.

![image](https://github.com/user-attachments/assets/898d1523-d33b-4fb0-b6a2-92e38f08cdcb)


Store 11 from department 54 is on a downward direction approaching zero in the new year.

![image](https://github.com/user-attachments/assets/482c9213-d735-41ea-94d5-1d955e02d668)



# 🛠️ 𝗧𝗼𝗼𝗹𝘀 𝗨𝘀𝗲𝗱

### 𝗗𝗮𝘁𝗮 𝗪𝗿𝗮𝗻𝗴𝗹𝗶𝗻𝗴: Python, Pandas
### 𝗘𝗗𝗔: Pandas
### 𝗗𝗮𝘁𝗮 𝗩𝗶𝘀𝘂𝗮𝗹𝗶𝘇𝗮𝘁𝗶𝗼𝗻s: Plotly Express
### Predictive Modeling: Prophet

If available more analysis to follow.

