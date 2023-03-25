# Algotrading
This is a support-vector machine based algotrading model which trains on a OHLCV dataset.

**3 Month SVC Classifier**

Initially, I trained the support vector machine on the 3 month period from April 2nd 2015 to July 2nd 2015. 
The decisions predicted from the classifier trained on this historical 3 month window were used to obtain predicted returns, which were then graphed alongside actual returns.

![svc_3-month](https://user-images.githubusercontent.com/54637095/226731265-c8059aed-2402-4a7a-92e2-9e84faa7d235.png)


**1 Month SVC Classifier**!

![svc_1-month](https://user-images.githubusercontent.com/54637095/226736032-5e6de8da-1ae7-420c-966d-1580cb7ab62f.png)

Reducing the historical training window from 3 months to a single month (April 2nd 2015 - May 2nd 2015) surprisngly doesn't affect our predictions too noticeably. There are few slight differences that are extremely subtle but probably not easy to pick up on at first glance.

**15 day SVC Classifier**!

![svc_15-day](https://user-images.githubusercontent.com/54637095/226741153-5d0d6825-72fc-4bc8-aa85-442b7897f6e6.png)


Interestingly, as we reduce the window even more, the area of the timeframe that sees differences between actual and predicted returns is sequestered more tho the right.


**6 Month SVC Classifier**

![svc_6month](https://user-images.githubusercontent.com/54637095/227732568-ea8fcbdb-4f51-41ee-9b92-9aac9124f69f.png)

By increasing the window, we see that the actual and predicted returns begin to diverge earlier. There's also in general more of a difference between the two quantities and it appears that the predicted returns at the 6 month window is actually worse for the most part than what is observed with the 3 month window

**6 Month Adaboost Classifier**

![ada_6-month](https://user-images.githubusercontent.com/54637095/227733953-b738b75e-bd73-4b83-b16f-a8dd0037655b.png)
