# Retail-Data-Analytics

## The aim of this project is to answer a few key questions. Which departments are leading in sales, which are the leading stores in those departments? The relationship between promotional markdowns and holidays and how that affects sales.



First thing we notice is the high amount of sales around 26th of November and 30 and 23-24 th December. While November 26 th is an official holiday in the United States 23rd of December is not but it is Christmas time so the high amount of sales that week makes sense.

![newplot](https://github.com/user-attachments/assets/e5aa2d9d-d972-46d4-90e1-a72baa0ee1a4)

Here we can see which days are officially holidays in the data. The week before and after December 31 st, there is huge drop in sales despite it being a holiday , suggesting a pattern of avoiding purchases by customers around the new year.

![newplot](https://github.com/user-attachments/assets/cfec1d07-69b3-46c6-ae2b-22db56bd3d66)


In this figure we can see the sales across departments and all 3 years. We can already see that some departments make much bigger share of the sales like number 92 , 95 , 38 , 72 , 40 and 2.

![newplot](https://github.com/user-attachments/assets/84e6ebae-1530-418d-ba2b-74441c1ddd33)


Here those top departments are selected and shown.

![newplot](https://github.com/user-attachments/assets/7073199f-5782-41aa-8ba8-c02b00ba7d23)



There was some really bad performing departmens in the data. The suprising thing was there is even one with negative amount of sales. Something mysterious is happening in Department 47. Sales in the nagative are not possible, recommendations are to check for fraud.

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

Since weekly sales data is available only until October 2012 and markdowns start from November 2011, we can see when plotted all together the effects Markdowns and Holidays are having on them. Particularly around the period of 25 November 2011 , from December 9 to December 30 - 2011 and around February 10 , 2012 and April 6 , 2012. Suprisingly even though there is a huge Markdown2 around December 30, 2011 and after , sales are dropping and quite low in that period.


![newplot](https://github.com/user-attachments/assets/3af6299a-5be6-4538-a2fd-83b179905290)


Predictive modelling using Prophet shows that sales will continue at the same pace until February 2013 with good accuracy and then the uncertainty becomes more with time.

![image](https://github.com/user-attachments/assets/1e45cf3a-7dae-42ea-9cc4-23b820306a92)


| Date       | yhat        | yhat_lower      | yhat_upper      |
|------------|-------------|-----------------|-----------------|
| 2012-11-11 | 17062.93    | -14874.91       | 49437.12        |
| 2012-11-18 | 17041.86    | -18056.25       | 47947.68        |
| 2012-11-25 | 17020.78    | -18913.65       | 51370.67        |
| 2012-12-02 | 16999.71    | -22080.88       | 54644.80        |
| 2012-12-09 | 16978.64    | -23030.39       | 56661.78        |
| 2012-12-16 | 16957.56    | -27128.20       | 62023.63        |
| 2012-12-23 | 16936.49    | -34019.85       | 60571.83        |
| 2012-12-30 | 16915.42    | -34425.86       | 65567.51        |
| 2013-01-06 | 16894.34    | -44453.70       | 70577.63        |
| 2013-01-13 | 16873.27    | -51705.45       | 76875.29        |
| 2013-01-20 | 16852.20    | -56951.70       | 81698.85        |
| 2013-01-27 | 16831.12    | -64702.79       | 93441.01        |
| 2013-02-03 | 16810.05    | -70092.90       | 98461.16        |
| 2013-02-10 | 16788.97    | -79844.26       | 104297.37       |
| 2013-02-17 | 16767.90    | -88554.46       | 114762.00       |
| 2013-02-24 | 16746.83    | -104201.47      | 121943.58       |
| 2013-03-03 | 16725.75    | -101575.37      | 124436.29       |
| 2013-03-10 | 16704.68    | -117340.08      | 140848.84       |
| 2013-03-17 | 16683.61    | -121484.06      | 155399.98       |
| 2013-03-24 | 16662.53    | -136876.76      | 156403.15       |
| 2013-03-31 | 16641.46    | -141588.00      | 166248.79       |
| 2013-04-07 | 16620.39    | -152581.10      | 170898.19       |
| 2013-04-14 | 16599.31    | -160975.16      | 185788.02       |
| 2013-04-21 | 16578.24    | -170704.89      | 196781.31       |
| 2013-04-28 | 16557.16    | -184095.06      | 210860.94       |
| 2013-05-05 | 16536.09    | -193997.97      | 219318.50       |
| 2013-05-12 | 16515.02    | -208671.85      | 238492.57       |
| 2013-05-19 | 16493.94    | -207477.11      | 243040.06       |
| 2013-05-26 | 16472.87    | -224552.37      | 257263.76       |
| 2013-06-02 | 16451.80    | -237355.73      | 269856.29       |
| 2013-06-09 | 16430.72    | -239407.82      | 285502.03       |
| 2013-06-16 | 16409.65    | -260294.09      | 294461.77       |
| 2013-06-23 | 16388.57    | -268248.24      | 310442.39       |
| 2013-06-30 | 16367.50    | -279254.48      | 326210.73       |
| 2013-07-07 | 16346.43    | -295528.33      | 336340.10       |
| 2013-07-14 | 16325.35    | -308865.98      | 346977.79       |
| 2013-07-21 | 16304.28    | -310691.02      | 370152.99       |
| 2013-07-28 | 16283.21    | -326955.46      | 380660.00       |


# 🛠️ 𝗧𝗼𝗼𝗹𝘀 𝗨𝘀𝗲𝗱

### 𝗗𝗮𝘁𝗮 𝗪𝗿𝗮𝗻𝗴𝗹𝗶𝗻𝗴: Python, Pandas
### 𝗘𝗗𝗔: Pandas
### 𝗗𝗮𝘁𝗮 𝗩𝗶𝘀𝘂𝗮𝗹𝗶𝘇𝗮𝘁𝗶𝗼𝗻s: Plotly Express
### Predictive Modeling: Prophet

If available more analysis to follow.

