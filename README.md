# Group-5-Project-1-MIST4610
## Team Name: 
21479 Group 5
## Team Members:
1. Simra Baig [@simrabaig](https://www.github.com/simrabaig)
2. Miranda Gonzalez [@mag93887](https://www.github.com/mag93887)
3. Matthew Wilbanks [@Mwilbanks22](https://www.github.com/Mwilbanks22)
4. Will Barrett[@Wbarrett1013](https://www.github.com/Wbarrett1013)
5. Terri Morrison [@terrimorrison28](https://www.github.com/terrimorrison28)

## Problem Description:
The problem we chose to address involves designing and constructing a relational database that models various aspects of sports at the University of Georgia. The central entity in our database is the Sports entity, which serves as the foundation for capturing data related to different sports at UGA. From this, we expand to include relevant details such as teams, players, coaches, games, and athlete performance. Our objective is to create a structured and efficient way to store and retrieve data, allowing for easy analysis and insights into multiple aspects of UGA athletics. Additionally, we aim to generate sample data, populate our database with realistic entries, and execute meaningful queries to extract valuable information regarding sports operations and trends at UGA.
## Data Model

Explanation of data model: 

This data model is based on the structure of UGA’s sports teams. The sports entity is representative of the UGA athletic aspects within each sport. Within each sport, there are teams that classify as a one-to-many non-identifying relationship. Each team has a donor, making this a one-to-many non-identifying relationship. Every sports team has coaches to guide and train the team to play to the best of their ability. This relationship is one-to-many and non-identifying. The entity coaches is a one-to-one non-identifying relationship itself. 

Each team includes many players who can play for one or multiple teams. That identifies as a one-to-many non-identifying relationship. Sports need players to be eligible for competition and games to play. This creates a one-to-many non-identifying relationship. Athletic performance is a one-to-many identifying relationship with the players entity and a one-to-many non-identifying relationship with coaches.

Athletic performances are recorded for each game played. This is a one-to-many non-identifying relationship. For every sport, there are multiple games for certain seasons and duration. These form a one-to-many non-identifying relationship. For every game, tickets are sold to fans and students for specific prices at specific games. 

Every sport there are staff members who help in their roles to support the sports teams.This forms a one-to-many non-identifying relationship. Each sport has to have facilities to host these games. The facilities entity keeps a record of location, capacity, and names. Finally, shared facilities is an identified many-to-many relationship between the sports and facilities entity. This records the number of usages of facilities by certain sports and the maintenance status.



![6A544222-9A29-45E3-B6C5-6FC7EEDA86ACImage 3-16-25 at 8 39 PM](https://github.com/user-attachments/assets/b036b55f-60bb-449b-add4-dce10d85133a)


## Data Dictionary:
<img width="695" alt="Screenshot 2025-03-17 at 8 50 46 PM" src="https://github.com/user-attachments/assets/d1a8be17-d500-41c9-8013-e6e924767f3a" />
<img width="691" alt="Screenshot 2025-03-17 at 8 51 14 PM" src="https://github.com/user-attachments/assets/d7436031-e07b-41d1-b903-1fbfc5334bba" />
<img width="688" alt="Screenshot 2025-03-17 at 8 51 33 PM" src="https://github.com/user-attachments/assets/355a6dbe-84eb-4107-9f3d-12b72153ebc2" />
<img width="690" alt="Screenshot 2025-03-17 at 8 51 45 PM" src="https://github.com/user-attachments/assets/d24cc725-a57a-43ed-8ef1-90e78a2d0dbb" />
<img width="706" alt="Screenshot 2025-03-17 at 8 52 08 PM" src="https://github.com/user-attachments/assets/8a9369c5-4cd7-4239-bf3f-a3907a502374" />
<img width="528" alt="Screenshot 2025-03-17 at 8 52 40 PM" src="https://github.com/user-attachments/assets/80aa8379-e920-4cd4-9ea9-d780f36c2232" />
<img width="523" alt="Screenshot 2025-03-17 at 8 52 56 PM" src="https://github.com/user-attachments/assets/32185e9d-d0be-4018-ab5c-c717b5ba1f1c" />
<img width="544" alt="Screenshot 2025-03-17 at 8 53 11 PM" src="https://github.com/user-attachments/assets/8f676cdb-c3ad-4dd9-8e07-b328efe65aca" />
<img width="532" alt="Screenshot 2025-03-17 at 8 53 21 PM" src="https://github.com/user-attachments/assets/558c3147-4004-414d-9c68-45245bd432f1" />
<img width="520" alt="Screenshot 2025-03-17 at 8 53 30 PM" src="https://github.com/user-attachments/assets/3fb1c7e1-4b96-4e62-98fc-f75349aa7448" />
<img width="530" alt="Screenshot 2025-03-17 at 8 53 44 PM" src="https://github.com/user-attachments/assets/e70a9e1d-7af0-4b1a-96e4-b181e47bd2b5" />

## Queries:

1. Query 1 lists out the names of all the players, ordered alphabetically


Query 1 allows allows managers to see which establishments have received the most number of reservations during their busiest time (6-8pm) which is typically dinner time. These establishments likely need more support, resources, and personnel around dinner time. Therefore, this query allows managers to identify which establishments to allocate this extra help to. Listing the results in descending order of number of reservations makes it easier to see which establishment to prioritize.

2. Query 2 lists the number of dining reservations made by guests on each floor. The results are ordered in ascending order of floor number.

![Screen Shot 2023-03-31 at 5 50 39 PM](https://user-images.githubusercontent.com/128402101/229239237-725cac35-598a-49e5-9b5d-bfc96fb18714.png)

Query 2 allows managers to see whether there is a trend between what floor a guest stays on and how much they reserve tabes at the resort's dining establishments. If managers were to find that dining reservations decreased as the floor number increased, it would have possibly indicated that guests were not dining at dining establishments because they felt the distance of the dining establishment from their room was too far and inconvenient.

3. Query 3 lists the information for all the guests who have not made an activity reservation.

![Screen Shot 2023-03-31 at 5 52 01 PM](https://user-images.githubusercontent.com/128402101/229239403-19acc956-7345-406e-b7ba-a6eaf1c8db88.png)

Query 3 allows the resort to market toward specific customers and contact them (e.g. promotional emails/coupons) about must-try activities. This helps to maximize revenue and increase efficiency by specifically targeting those who are not engaging in activities, rather than wasting time and resources to advertise to those who are already aware of and partaking in these activities.

4. Query 4 lists the names and phone numbers of dining employees who work in the highest rated dining establishment.
 
![Screen Shot 2023-03-31 at 5 53 30 PM](https://user-images.githubusercontent.com/128402101/229239730-7f5416bd-0aff-4c4a-b64d-7f365f246a36.png)

A restaurant with a high star rating is a large source of revenue for the resort and management may want to know the names of the employees who work there and how to contact them to reward them for maintaining such a high achieving restaurant (e.g. via a bonus, raise, awards, recognition) or to know which employees to target for continuous training and supervision in order to keep service within the establishment in top shape.

5. Query 5 lists the guests’ names and the hotel they are checking into if their reservation is during the PM, their room is a single or suite, their check in dates are between 2023-04-01 and 2023-04-10, and their hotel rating is above a 4.

![Screen Shot 2023-03-31 at 5 54 41 PM](https://user-images.githubusercontent.com/128402101/229239947-e3c0ab47-c77c-474b-81c1-1b187548b89c.png)

Query 5 allows the resort to manage how busy their check in will be during the PM hours of early April in their better hotels where the check in rooms are singles or suites. This can help the resort determine how many employees need to be working the check in desks to check in single or suite reservations in the afternoon of these dates in these specific hotels.

6. Query 6 lists the names of guests who have over 10 activity reservations and the activities that they have those reservations in.

![Screen Shot 2023-03-31 at 5 55 37 PM](https://user-images.githubusercontent.com/128402101/229240045-10ca60c7-1cb2-49e2-a224-256c841e5fd8.png)

Query 6 allows the resort to determine what guests are contributing the most to each activity’s revenue. The resort may use this information to reward guests who spend the most on activities by offering special prizes and promotions, creating guest loyalty and creating an incentive to reserve even more.

7. Query 7 lists the the amount of dining reservations per guest and the average amount of guests these reservations have.

![Screen Shot 2023-03-31 at 5 56 06 PM](https://user-images.githubusercontent.com/128402101/229240108-152740f1-4c85-4a38-9194-c981cf33fc42.png)

Query 7 allows the resort to see how many guests they should plan to seat, how the tables should be set up, and can lead to the resort figuring out how much revenue should be expected for the average visit.

8. Query 8 lists the guestID, guest name, and the number of room reservations per guest.

![Screen Shot 2023-03-31 at 6 34 05 PM](https://user-images.githubusercontent.com/128402101/229244470-c29f68b3-f837-4a18-97bb-f86345b84431.png)

Query 8 allows the resort to identify their frequent customers and how many times they have stayed. This could lead to a card system down the line. If a guest reaches 5 or 10 visits, there could be a platinum card which would gift the user reservation priority, food discounts, and other perks.

9. Query 9 lists all the rooms along with their average room view rating if the rating is above a 4 star. Additionally, the query is sorted by the view rating and arranged in descending order.

![Screen Shot 2023-03-31 at 5 56 31 PM](https://user-images.githubusercontent.com/128402101/229240166-bb0bc849-08dd-4521-8608-7a85ff53ae46.png)

Query 9 allows the employees and customers to see which rooms have an average view rating of 4 or more. Rooms with extravagant views are huge attractions to customers and can be a deciding factor when picking which room to stay in. This will help employees find which rooms have the best views fast and efficiently when asked.

10. Query 10 lists the names and prices of all activities offered by the resort that have not yet been booked by any guests and that are less than or equal to $50. Additionally, the results of the query are ordered by price in ascending order.

![Screen Shot 2023-03-31 at 5 57 00 PM](https://user-images.githubusercontent.com/128402101/229240218-c01fb32b-5f71-4562-b014-b656bfe051bb.png)

Query 10 allows the employees and customers to see what activities have not been booked yet, and the prices for these activities. The price is sorted in ascending order to make it easier to find the most affordable activities which most people are looking for. Activities are a huge part of the resort experience and using this script will make it easy for employees to find which activities are available as well as the prices for these activities.

## Database information:

Name of the database: ns_Sp25_21479_Group5

Additional information: Each query listed above is marked in the database using stored procedures which can be called using the following format: 
CALL TP_Q01();
