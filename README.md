# On Time Deliver KPI

### 1. Introduction
In 2020, my company failed 1 of their 19 Operational KPI. Fortunately we met the rest of it, which save us some trouble. But what if we had failed another one? You can be sure that penalties would have been applied... <br/>
Let's take a deeper look at what caused the "On Time Delivery" KPI to fail, so we can take concrete actions and meet the target this year.

### 2. Problem statement
Every shipment sent to a consignee is recorded in our system, alongside with a "REMARKS" column indicating what was the reason of delay, if any. We will go through the delayed shipment and analyzed the different justifications.

### 3. Reading the data
The KPI data is clustered by month. We need to load every sheet corresponding to each month and then combine them into 1 dataframe. 

![Settings Window](https://github.com/BriceChivu/On_Time_Delivery_KPI/blob/main/Pictures/fig1%20On%20Time%20Delivery%20KPI%20reading%20the%20data.png) 

### 4. Analysis
Now, we can look into the delayed shipment and start analyzing the reasons.
First, we need to select only the shipment being delayed and having a remark associated. This new dataframe will be named df_KPI_rem.
Then, we will cluster, standardize and finally plot the different reasons. 

![Settings Window](https://github.com/BriceChivu/On_Time_Delivery_KPI/blob/main/Pictures/fig%202%20Analysis%20On%20Time%20Delivery%20KPI.png) 

![Settings Window](https://github.com/BriceChivu/On_Time_Delivery_KPI/blob/main/Pictures/fig%203%20On%20Time%20Delivery%20plot%201%20with%20early%20cargo.png)

After discussion with the Customer Service officer in charge of handling the communication with the client on those issues, I understood that the reason "early cargo" actually means "early released of the shipment" (also called cargo), which is not considered as a delayed shipment. We will therefore remove this justification. <br/>
The below plot shows the different justifications of the delay shipments **caused by my company** (which resulted in the KPI failure).

![Settings Window](https://github.com/BriceChivu/On_Time_Delivery_KPI/blob/main/Pictures/fig%204%20On%20Time%20Delivery%20plot%202%20without%20early%20cargo.png)

Let's breakdown the different reasons to understand how the company can improve moving forward.

![Settings Window](https://github.com/BriceChivu/On_Time_Delivery_KPI/blob/main/Pictures/fig%204%20On%20Time%20Delivery%20plot%202%20without%20early%20cargo.png)

### 5. Conclusion
