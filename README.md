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

Every sport there are staff members who help in their roles to support the sports teams. This forms a one-to-many non-identifying relationship. Each sport has to have facilities to host these games. The facilities entity keeps a record of location, capacity, and names. Finally, shared facilities is an identified many-to-many relationship between the sports and facilities entity. This records the number of usages of facilities by certain sports and the maintenance status.



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
<img width="1101" alt="Screenshot 2025-03-17 at 9 17 43 PM" src="https://github.com/user-attachments/assets/ed8793cd-12e2-4838-97f5-ffe9402bb208" />

This query provides a way to retrieve all player names in alphabetical order, making it easier for sports analysts, coaches, and staff to locate specific players in an efficient manner. Organizing data in a readable format helps with things like roster management, and team evaluations, and helps retrieve a player's information. This query will also be beneficial for generating reports to ensure consistency in data presentation and will aid in administrative functions related to UGA Athletics.

2. Query 2 lists the names of players whose height and weight are greater than the average height and weight of all players.
<img width="1098" alt="Screenshot 2025-03-17 at 9 24 03 PM" src="https://github.com/user-attachments/assets/4320392e-e094-4825-aeb5-1c86daa56be6" />
This query helps identify players who are above average in both height and weight, which can be useful for coaches and sports analysts when assessing physical attributes and the relationship to player performance. This data can also be used to analyze trends in player physique across different sports at UGA, supporting training and recruitment decisions.


3. Query 3 List the number of tickets sold for each event and the total revenue for that sport. We then list the total revenue in desc order.

<img width="1080" alt="Screenshot 2025-03-17 at 9 25 43 PM" src="https://github.com/user-attachments/assets/8cd25c85-5a8a-4bea-9ce1-746a75df5d47" />

Query 3 This allows us to see how profitable each sport is as well as how popular the sport is based on ticket sales. Listing the results in desc order allows us to more efficiently examine the data.


4. Query 4 List out the names of teams and the number of players per team. Order by team names alphabetically

 <img width="1101" alt="Screenshot 2025-03-17 at 9 26 08 PM" src="https://github.com/user-attachments/assets/bcefea32-60b9-47f7-98b8-6b8cf64ec1ca" />

Query 4 allows us to see how many players are on each team by the actual team name. We order the team names alphabetically to make the results more readable.

5. Query 5 lists out the facilities that UGA owns that have a minimum of 5,000 seats.

<img width="1093" alt="Screenshot 2025-03-17 at 9 26 27 PM" src="https://github.com/user-attachments/assets/60e82a8e-a0ef-4a0f-8b26-08c2c0728e34" />


Query 5 allows for the University of Georgia Athletics to filter out some of the smaller athletic venues from the data.  UGA Athletics can use this information to make decisions based on the facilities that are used the most in order to try and boost the overall spectator experience to maximize the value that UGA Athletics produces.

6. Query 6 List out the teams with donors that are greater than the average donor amount per team. 

<img width="1097" alt="Screenshot 2025-03-17 at 9 26 45 PM" src="https://github.com/user-attachments/assets/45948bfb-dcc8-40d3-8032-188243b22890" />


Query 6 allows for UGA Athletics to see the sports and teams that are receiving an above average amount of donations to said sport / team.  UGA can use this information to make decisions on where to invest money into each sport and team based on how much a team is receiving and either further invest or decide to invest into another sport to insure that each sport is being treated fairly. 

7. Query 7 lists out the team’s name, opponent, date, and location where the result of the game was a win.
   
![022F1F98-369E-47AF-A521-C86135CAFA3F](https://github.com/user-attachments/assets/c59afe1b-27d7-4673-93bf-dd27376c7158)


Query 7 allows individuals to track team performance by displaying each team's name, opponent, game date, and location for games that resulted in a win. If people discover that a team wins more often at home than away, it may indicate a home-field advantage, implying that variables such as fan support, familiarity with the facility, or less travel fatigue contribute to improved performance.

8. Query 8 lists out the names of coaches and the names of players they coach.
   
![3434D765-3EAB-4A53-B7E0-DAD8BF183FC3](https://github.com/user-attachments/assets/165e0493-0c82-4f54-bf21-2aa58258e09c)


Query 8 helps individuals identify the relationship between coaches and the athletes they train by listing each coach's name next to their players' names. If individuals discover that particular coaches typically have more players or work with higher-performing athletes, it may imply disparities in coaching efficiency, training methods, or recruitment techniques that influence player development and team performance.

9. Query 9 lists all the rooms along with their average room view rating if the rating is above a 4 star. Additionally, the query is sorted by the view rating and arranged in descending order.
    
<img width="1101" alt="Screenshot 2025-03-17 at 9 27 52 PM" src="https://github.com/user-attachments/assets/3e458371-7fc9-4ed4-b5ff-eb2f1c77c1af" />

Query 9 allows the employees and customers to see which rooms have an average view rating of 4 or more. Rooms with extravagant views are huge attractions to customers and can be a deciding factor when picking which room to stay in. This will help employees find which rooms have the best views fast and efficiently when asked.

10. Query 10 lists the names and prices of all activities offered by the resort that have not yet been booked by any guests and that are less than or equal to $50. Additionally, the results of the query are ordered by price in ascending order.

<img width="1097" alt="Screenshot 2025-03-17 at 9 28 16 PM" src="https://github.com/user-attachments/assets/bdcfe8ed-f6c7-4595-9c84-d0aeee826242" />

Query 10 allows the employees and customers to see what activities have not been booked yet, and the prices for these activities. The price is sorted in ascending order to make it easier to find the most affordable activities which most people are looking for. Activities are a huge part of the resort experience and using this script will make it easy for employees to find which activities are available as well as the prices for these activities.

## Database information:

Name of the database: ns_Sp25_21479_Group5

Additional information: Each query listed above is marked in the database using stored procedures which can be called using the following format: 
CALL TP_Q01();
