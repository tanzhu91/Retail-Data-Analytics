# Retail-Data-Analytics



First thing we notice is the high amount of sales around 26th ov November and 30 and 23-24 th December. While November 26 th is an official holiday in the United States 23rd of December is not but it is Christmas time so the high amount of sales the week before that makes sense.

![newplot](https://github.com/user-attachments/assets/e5aa2d9d-d972-46d4-90e1-a72baa0ee1a4)

Here we can see which days are officially holidays in the data. The week before December 31 st, there is huge drop in sales despite it being a holiday , suggesting a pattern of avoiding purchases by customers right before the new year.

![newplot](https://github.com/user-attachments/assets/cfec1d07-69b3-46c6-ae2b-22db56bd3d66)


In this figure we can see the sales across departments and all 3 years. We can already see that some departments make much bigger share of the sales like number 92 , 95 , 38 , 72 , 40 and 2.

![newplot](https://github.com/user-attachments/assets/84e6ebae-1530-418d-ba2b-74441c1ddd33)


Here those top departments are selected and shown.

![newplot](https://github.com/user-attachments/assets/7073199f-5782-41aa-8ba8-c02b00ba7d23)



There was some really bad performing departmens in the data. The suprising thing was there is even one with negative amount of sales. Something mysterious is happening in Department 47.

![newplot](https://github.com/user-attachments/assets/40f9279d-d689-4640-a00d-37b013e08181)


Here Weekly sales are plotted against type of stores and amount of sales based on holiday or not.

![newplot](https://github.com/user-attachments/assets/d74e29e3-5157-4309-a883-36a6cce93779)



I decided to plot the stores of the best performing department based on sales and the worst one. We can see that department 92 has best performing stores numbered as follows: 14,2,20,13,4 and so on. The size is not always the biggest but most of them are close to the biggest possible.

![newplot](https://github.com/user-attachments/assets/06380c5a-8280-4816-b98c-67305e308455)


Worst performers in department 47 are store number 35,1,10,45 and so on.

![newplot](https://github.com/user-attachments/assets/1d8e61da-1c5d-43fc-9f63-d88b9f3602aa)



Here correlation between size of stores and weekly sales shows clearly there is a positive relationship. The bigger the store the more sales in total. The model is with an R value of 71 % , so it is quite good.

![newplot](https://github.com/user-attachments/assets/d9fd3189-a5d0-42d4-bdc7-7efca57fea60)


In this graph we can see the dates when promotional markdowns were available. A lot of them are right before holidays or around holiday times.

![newplot](https://github.com/user-attachments/assets/d6079831-c44c-4fe3-a57c-80245bf9e43e)

And here we can see the correlation between markdowns and holidays.

![newplot](https://github.com/user-attachments/assets/e6fd74c7-927e-4943-8475-d6efe3b1facd)


Predictive modelling shows that sales will continue at the same pace until February 2013 with extreme accuracy and then it gets less accurate with time.

![image](https://github.com/user-attachments/assets/b7d48d4e-91c9-4453-9bd9-ed4e85677b3b)

      date         yhat         yhat_lower     yhat_upper
50 2012-11-11  17062.932356  -14874.911979   49437.122910
51 2012-11-18  17041.858674  -18056.249778   47947.681672
52 2012-11-25  17020.784992  -18913.653323   51370.671329
53 2012-12-02  16999.711311  -22080.875210   54644.800123
54 2012-12-09  16978.637629  -23030.389169   56661.777037
55 2012-12-16  16957.563947  -27128.197449   62023.629759
56 2012-12-23  16936.490265  -34019.851474   60571.830743
57 2012-12-30  16915.416583  -34425.857911   65567.509637
58 2013-01-06  16894.342901  -44453.701380   70577.634757
59 2013-01-13  16873.269219  -51705.451131   76875.287225
60 2013-01-20  16852.195538  -56951.702756   81698.850350
61 2013-01-27  16831.121856  -64702.785497   93441.011193
62 2013-02-03  16810.048174  -70092.901798   98461.159219
63 2013-02-10  16788.974492  -79844.259691  104297.367154
64 2013-02-17  16767.900810  -88554.462536  114762.000120
65 2013-02-24  16746.827128 -104201.467588  121943.579873
66 2013-03-03  16725.753446 -101575.373050  124436.285294
67 2013-03-10  16704.679764 -117340.083833  140848.840258
68 2013-03-17  16683.606083 -121484.055853  155399.981955
69 2013-03-24  16662.532401 -136876.761416  156403.154168
70 2013-03-31  16641.458719 -141587.977525  166248.786695
71 2013-04-07  16620.385037 -152581.097504  170898.187342
72 2013-04-14  16599.311355 -160975.157417  185788.022614
73 2013-04-21  16578.237673 -170704.888180  196781.314105
74 2013-04-28  16557.163991 -184095.062389  210860.943887
75 2013-05-05  16536.090310 -193997.967397  219318.498182
76 2013-05-12  16515.016628 -208671.853034  238492.569087
77 2013-05-19  16493.942946 -207477.111004  243040.058910
78 2013-05-26  16472.869264 -224552.374369  257263.759218
79 2013-06-02  16451.795582 -237355.734823  269856.287940
80 2013-06-09  16430.721900 -239407.817224  285502.034600
81 2013-06-16  16409.648218 -260294.094720  294461.767587
82 2013-06-23  16388.574536 -268248.235962  310442.392167
83 2013-06-30  16367.500855 -279254.476344  326210.734167
84 2013-07-07  16346.427173 -295528.331812  336340.102365
85 2013-07-14  16325.353491 -308865.976007  346977.789457
86 2013-07-21  16304.279809 -310691.022225  370152.989074
87 2013-07-28  16283.206127 -326955.457105  380660.003353




If available more analysis to follow.

