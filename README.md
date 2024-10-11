This is a transaction level data at the Rogers market with Amazon Just Walk Out technology at Feb. 28, 2024. 

Key columns that will be used in this homework:

Purchase_datetime: It is a purchase time. Consider it as an exit time from the store.

Session_id: It is a session identifier, i.e., the first three transactions are three items that *ONE* group of size 1 bought. Notice that those three transactions have the same purchase_datetime.

Trip_duration_mins: It is how long a customer/a group of customers spend within the store. So, purchase_datetime - trip_duration_mins = an entry time to the store.

Group_size: how many customers came into the store as a group. One customer in that group will pay all together.

1- Plot how many customers entered the store in every 15 minutes from 7AM-11:00PM. Then, calculate how many customers entered the store per hour on average.

2- Take the average of trip_duration_mins, considering the group size. What is the average flow time of a customer, i.e., on average, how many minutes a customer spends in the store?

3- From 7AM till 11PM, draw the inventory build-up diagram. 

4- Calculate the total time summed up over all customers, i.e., the area under the inventory build-up diagram. Then, calculate the Inventory (or, the average inventory).

5- Check the Little’s Law using the answers from above.
