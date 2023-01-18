# Laptop_cost_prediction



## EDA 


### Distribution Plot of our dependent feature Price.
![plot1](https://user-images.githubusercontent.com/67755812/213108818-453cec2f-a66c-4cd9-83ef-8a440cdbb8e1.png)

### As we can see the distribution it is little a bit a left skewed Gaussian Distribution.



## Plotting the countplots of categorical Variables

### Companies Selling Laptops
![company_plot2](https://user-images.githubusercontent.com/67755812/213109042-8986b58b-b66c-45ed-a98d-c682b1740507.png)

## HP as around 275 laptops out of 1303. Whereas Dell and Lenovo has crossed the HP with 290 approx laptops out of 1303. We see that the least is with google, LG, Fujitsu, Huawei, etc



### Laptop types
![typename_plot2](https://user-images.githubusercontent.com/67755812/213109601-7339ed3f-a751-4307-9af5-3705774adb59.png)

### And we have the what kind of models are sold mostly Notebooks followed by Ultrabook and Gaming. The least models sold are netbook and workstation.

## RAM
![ram_plot2](https://user-images.githubusercontent.com/67755812/213109710-8090f789-4af7-4738-838b-4141776706a5.png)

## Operating System
![opsys_plot2](https://user-images.githubusercontent.com/67755812/213109749-c8f8b44e-3d25-4178-b3fe-7b4fabe7af33.png)

## Compnay VS Price
![company_vs_price](https://user-images.githubusercontent.com/67755812/213114831-cb2dda0f-6a26-4bd7-b29c-86320b506e82.png)

Then we will see average price for each laptop brand. It will give us the insight how the price of laptop will vary.
According to the dataset, We can see the ticks at boxplot of HP the maximum (avg) selling price it goes to 65K - 70K (It can be  more but the dataset does not contain that data) and average selling would be to 50K- 52K. For Apple the maximum (avg)selling price it goes to approx 1Lac (It can be  more but the dataset does not contain that data) and average selling would be to 65K- 70K. So we can a lot variations of price, so we get to know what is the average variation of a company's laptop and what can be maximum price which a company can assign to its laptop.



## Laptop Type VS Price
![plot4](https://user-images.githubusercontent.com/67755812/213109826-273c8058-0168-489e-bac1-5065cadad144.png)

In the above plot, we get to know that notebook does not have that much price variation. maybe beacuse the notebooks are used for general purpose so that it can be scalable to peoples. 



##  ScreenSize_Price
![plot5](https://user-images.githubusercontent.com/67755812/213109863-30c68d9a-91d2-42e0-877c-75668a56a99e.png)

In the plot, we observe that the most of the people buys laptops with screensize around 13 - 14 inches. While the laptops with screensize of 17inches are sold upto 3Lakhs or more. Also, most people buys laptop with screensize of 15.6 inches and we can see some scatter over the 15.6 so we can say that the data is almost right.

<hr>

### For the Screen Resolution column we have many types of Screen Resolutions out there as shown Touch Screen and Normal and IPS Panel are the 3 parts on basis of which we can segregate the things

Full HD 1920x1080                                507
1366x768                                         281
IPS Panel Full HD 1920x1080                      230
IPS Panel Full HD / Touchscreen 1920x1080         53
Full HD / Touchscreen 1920x1080                   47
1600x900                                          23
Touchscreen 1366x768                              16
Quad HD+ / Touchscreen 3200x1800                  15
IPS Panel 4K Ultra HD 3840x2160                   12
IPS Panel 4K Ultra HD / Touchscreen 3840x2160     11
4K Ultra HD / Touchscreen 3840x2160               10
Touchscreen 2560x1440                              7
4K Ultra HD 3840x2160                              7
IPS Panel 1366x768                                 7
IPS Panel Quad HD+ / Touchscreen 3200x1800         6
Touchscreen 2256x1504                              6
IPS Panel Retina Display 2560x1600                 6
IPS Panel Retina Display 2304x1440                 6
IPS Panel Touchscreen 2560x1440                    5
IPS Panel 2560x1440                                4
IPS Panel Retina Display 2880x1800                 4
1440x900                                           4
IPS Panel Touchscreen 1920x1200                    4
2560x1440                                          3
1920x1080                                          3
IPS Panel Quad HD+ 2560x1440                       3
IPS Panel Touchscreen 1366x768                     3
Touchscreen 2400x1600                              3
Quad HD+ 3200x1800                                 3
IPS Panel Full HD 2160x1440                        2
IPS Panel Quad HD+ 3200x1800                       2
IPS Panel Touchscreen / 4K Ultra HD 3840x2160      2
Touchscreen / Full HD 1920x1080                    1
Touchscreen / Quad HD+ 3200x1800                   1
Touchscreen / 4K Ultra HD 3840x2160                1
IPS Panel Full HD 1920x1200                        1
IPS Panel Full HD 2560x1440                        1
IPS Panel Retina Display 2736x1824                 1
IPS Panel Touchscreen 2400x1600                    1
IPS Panel Full HD 1366x768                         1


So now will be creating a new col,touchscreen if the value is 1 that laptop is touch screen

![resolution_code](https://user-images.githubusercontent.com/67755812/213109919-58559d06-1b8f-411b-9754-4f4ee0869ca7.PNG)

![data_image](https://user-images.githubusercontent.com/67755812/213109947-82c55f63-d1fd-45bc-ab9b-fdc5fd568281.PNG)

### Count of TouchScreen Laptops
![plot 6](https://user-images.githubusercontent.com/67755812/213115895-52c0b5ff-c91b-4daf-8772-65fb735a09ce.png)

#### So using countplot, we get to know that almost 190 laptops are touchscreen and rest of all laptops are not touchscreen.

### TouchScreen VS Price
![plot7](https://user-images.githubusercontent.com/67755812/213110046-767aaace-385f-43f3-a7bd-0c726a1b59c6.png)

#### The price for touchscreen laptops are the highest 80k or it can go more than 80k and average pricr is 70K.

<hr>

### So now will be creating a new col for ips panel as well  if the value is 1 that laptop is touch screen
![ips_image](https://user-images.githubusercontent.com/67755812/213110081-74c90681-5ac1-4bbe-a8f1-1e27b8996bed.PNG)

![ips_data_image](https://user-images.githubusercontent.com/67755812/213110115-b31a8bbd-f262-4746-8a95-ad714e1331d0.PNG)


### IPS Panel count
![plot8](https://user-images.githubusercontent.com/67755812/213110142-6295b556-a047-4012-adc2-d5f83e0177f3.png)

#### So using countplot, we get to know that almost 350 - 400 laptops are IPS and rest of all laptops are not IPS


### Panel VS Price
![plot9](https://user-images.githubusercontent.com/67755812/213110168-f02842f6-74b8-4062-aa0c-e1b150358b0b.png)

#### The price for touchscreen laptops are the highest 80k  and average price is 65K.

<hr>

## Correlation

![plot10](https://user-images.githubusercontent.com/67755812/213110200-943d7409-ad06-4dea-a95d-e0fddae0e335.png)

![corr1_image](https://user-images.githubusercontent.com/67755812/213110229-e26fb6b3-01b7-48a8-880c-7e6ccda2cdd5.PNG)

From the correlation plot we observed that as the X_res and Y_res is increasing,the price of the laptop is also increasing,so `X_res and Y_res` are positively correlated and they are giving much information,so that is the reason why i had splitted `Resolution` column into `X_res and Y_res` columns respectively.So to make things good,we can create a new column named PPI{pixels per inch},now as we saw from the correlation plot that the X_res and Y_res are having much collinearity,so why not combine them with Inches which is having less collinearity,so we will combine them as follows ↓,so here is the formula of how to calculate PPI {pixels per inch}.

![ppi](https://user-images.githubusercontent.com/67755812/213117335-a606fc60-b3bf-411f-88ba-e859b02b8ec4.PNG)


![corr2_image](https://user-images.githubusercontent.com/67755812/213110280-479957d4-706f-4dad-8272-087658db58c7.PNG)

So as we observe from the correlation data that the PPI is having good correlation,so we will be using that,as that is a combination of 3 features and that gives collective results of 3 columns,so we will drop Inches,X_res,Y_res as well


<hr>

## Now we will work on `CPU` column,as that also has much text data and we need to process it efficiently as we may get good insights from them

Most common processors are made by intel right,so we will be clustering their processors into different categories like i5,i7,other,now other means the processors of intel which do not have i3,i5 or i7 attached to it,they're completely different so that's the reason i will clutter them into other and other category is AMD which is a different category in whole

So if we observe we need to extract the first 3 words of the CPU column,as the first 3 words of every row under the CPU col is the type of the CPU,so we will be using them as shown 

![plot11](https://user-images.githubusercontent.com/67755812/213110307-cc009af1-446d-45a2-aa9d-63f601979cd8.png)

#### we see that i5 is around 430-440, and i7 are around more than 500

![plot12](https://user-images.githubusercontent.com/67755812/213110320-8b185720-bca4-4ce5-949e-f6f3f0a4e57a.png)


## Analysis on RAM

![plot13](https://user-images.githubusercontent.com/67755812/213110340-f0a1b7e4-6cd8-4a60-9918-2ec454ce62c7.png)
#### We can see that more than 600 uses 8gb ram and other major quantity is 4gb ram and we find few people who prefer 16gb ram 


![plot14](https://user-images.githubusercontent.com/67755812/213110384-70f845af-074d-44d6-8bfc-912c65262b09.png)
#### RAM is having good relation with price

<hr>

## Memory Column
We will seperate the `Type` of memory and the value of it,just similar to the one which is done in the previous part

This part involves things which are needed to be done in steps,so here we do not have the memory as a complete we have it in different dimension as `128GB SSD +  1TB HDD`,so inorder to for it come in a same dimension we need to do some modifications which are done below as shown


![corr_image3](https://user-images.githubusercontent.com/67755812/213110471-65af958d-6273-4b3e-9798-c337f5e5ac73.PNG)

Based on the correlation we observe that Hybrid and Flash Storage are almost negligible,so we can simply drop them off,where as HDD and SDD are having good correlation,we find that HDD has -ve relation with Price,and that's true,if the price of laptop is increasing there is more probability that the laptop is gonna use SDD instead of HDD and vice versa as well


<hr>

## Analysis on GPU

### Here as we are having less data regarding the laptops,its better that we focus on GPU brands instead focusing on the values which are present there beside them,we will focus on the brands

![plot15](https://user-images.githubusercontent.com/67755812/213110502-2dee5364-f64b-4dc0-9cab-1468dac8040a.png)

![plot16](https://user-images.githubusercontent.com/67755812/213110518-837ba48c-86fa-444a-9eb5-def9f5e3ca20.png)

### Removing the "ARM" tuple

![plot17](https://user-images.githubusercontent.com/67755812/213110550-2b59a6a7-8f71-4e62-96ee-411468291682.png)


<hr>

## Operating System Analysis

![plot18](https://user-images.githubusercontent.com/67755812/213111109-11ed0e0a-f4a5-463f-9e8f-e9d70d9f5274.png)

### Grouping all Windows version into Windows and all Mac versions into Mac OS

![plot19](https://user-images.githubusercontent.com/67755812/213111136-3549bd40-e4b6-49a0-b82b-314c43492d56.png)

![plot20](https://user-images.githubusercontent.com/67755812/213111152-0ab5bb21-81b3-4cfd-979d-3ef13cc49f6c.png)



<hr>


## Laptop Weight analysis

![plot21](https://user-images.githubusercontent.com/67755812/213111183-10fef0fb-6509-4c53-923a-e00a734a26fe.png)

![plot22](https://user-images.githubusercontent.com/67755812/213111205-af8593ab-3cf8-42d1-af2c-b74d0271f4a2.png)

<hr>

## Price Analysis
![plot23](https://user-images.githubusercontent.com/67755812/213111232-2d19a086-9c36-4a88-8af3-9e52b7263852.png)

### As we can see that the plot is kind of left skewed.

![plot24](https://user-images.githubusercontent.com/67755812/213111261-51f9ff4c-2573-4d21-b077-5813a9a56369.png)

### So we apply log to the price and it become centrally distributed (Gaussian)

 # --------------------------------------Models-----------------------------------

## We will be using Pipelines to load the model

## Regression Models

## Linear Regression
Step 1 would be to convert categorical values to Numerical Values
Step 2 is like an object of the model

![linear_reg](https://user-images.githubusercontent.com/67755812/213111897-0b970c70-13a5-4a37-b7fe-8b8212b3d4e1.PNG)

### R2 score 80.73%
### MAE 0.2101783


## Ridge Regression
![ridge_reg](https://user-images.githubusercontent.com/67755812/213113398-f8543b91-ca58-4447-a51a-9fcbf3075952.PNG)

### R2 score 81.27%
### MAE 0.2092680


## Lasso Regression
![lasso_reg](https://user-images.githubusercontent.com/67755812/213113529-e0870ee8-34be-418e-bf70-4a8c49366dff.PNG)

### R2 score 80.71%
### MAE 0.2111435

##  Ensemble Models

## Decision Tree

![decision_tree](https://user-images.githubusercontent.com/67755812/213118553-5f867e78-033f-4d83-b4a0-9fc8e6b82256.PNG)

### R2 score 84.33%
### MAE 0.1830225

## Random Forest

![random_forest](https://user-images.githubusercontent.com/67755812/213118602-ffcd7bea-350f-4bdd-b96e-d0b6f5695162.PNG)

### R2 score 90.82%
### MAE 0.1587025

## Checking how Random Forest Model predicts the value wrt to Actual value.

![actual_pred](https://user-images.githubusercontent.com/67755812/213121559-a9d51323-063b-4881-95b3-b1ef7d4df77a.png)

<hr>

# Conclusion: 
Random Forest model gives best score from the above all Models. So we will be using Random Forest Model for Web App. 

## Note: I also worked on Hyperparameter Tunning of Random Forest but after tunning the model is giving us the same score.


