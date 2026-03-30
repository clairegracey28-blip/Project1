# Team 6 MIST 4610 Group Project1

## Team Name:
21479 Group 6

## Team Members:
  1. Tobi Alaba
  2. Claire Gracey
  3. Naysa McFarlane
  4. Andy Smith

## Problem Description:   
  Problem: Create and build a relational database of a mock 'Major League Volleyball' database to demonstrate relationships between the volleyball league of teams, coaches, tournaments, players, etc. The central entity is the team entity of the volleyball league, displaying multiple relationships to find team specifics, such as name and location. Overall, the goal is to accurately model these relationships by generating sample data and populating each entity and its attributes with relevant sample data from Mockaroo. Furthermore, we aim to enable simple and complex querying of big sample data for team analysts, coaches, administrators, and other relevant stakeholders. This can show valuable operational and performance insights about teams or the league as a whole.

## Data Model:   **NOT FINISHED**
  Data Model Description:  
  
  Our data model is primarily based on a hypothetical volleyball league, called the MLV (Major League Volleyball). The data model is centered around the team entity. The team entity represents the numerous teams within the MLV. The team entity has many branches stemming from it, with the first being the player entity. Each team has many players, signifed by the one-to-many relationship between the team entity and the player entity.

  Each player can have none, one, or multiple injuries, thus the one-to-many relationship between the player entity and the previousInjuries entity. Each player can also have multiple exercise evaluations, where they are evaluated to determine athletic ability, therefore the one-to-many relationship between player and exerciseEvaluation. 

  Going back to the team entity, a team typicall has one roster, and a specific roster is only associated with one team, so a one-to-one relationship exists between the team entity and the roster entity. Further, each roster belongs to one coach, and one coach belongs to each roster, thus another one-to-one relationship is formed, this time between the roster entity and the coach entity. As we know, a coach coaches many players, and a roster contains multiple players as well, so a one-to-many relationship exists between both the roster entity and player entity, as well as the coach entity and the player entity.

  On any given team, there are multiple staff members, but staff members only belong on one specific team, so a one-to-many relationship exists from the team entity to the staff entity.

  For a team to succeed financially, they will typically need a sponsor. In our example, each team will only have one sponsor, and each sponsor will only sponsor one team. This creates a one-to-one relatioship between the team entity and the sponsors entity.

  During any given match, two teams play each other. Each team will play in many matches throughout the season, but each match will be played between two specific teams. In order to get the two unique teamID's, we have established two unique one-to-many relationships stemming from the team entity to the match entity. This shows the specific two teams that played in any given match, at any point in the season.

  Each match is won when either team wins multiple sets. That being said, each set will only be won in one specific match. This creates a one-to-many relationship between the match entity and the set entity.

  In addition to the regular season, there are tournaments throughout the season. Each team will play in many tournaments throughout the season, and each tournament consists of many teams. 

<img width="576" height="732" alt="Screenshot 2026-03-29 at 9 58 50 PM" src="https://github.com/user-attachments/assets/dfbdeeee-23e1-4f61-a8c5-ea48d20082c7" />


## Data Dictionary
<img width="650" height="328" alt="Screenshot 2026-03-29 at 4 29 38 PM" src="https://github.com/user-attachments/assets/d160e310-abe0-42e7-b6e5-6a6c9019bf70" />

<img width="640" height="416" alt="Screenshot 2026-03-29 at 4 30 45 PM" src="https://github.com/user-attachments/assets/f8f18307-e54e-44d1-a67f-59aa04968589" />

<img width="647" height="565" alt="Screenshot 2026-03-29 at 4 34 24 PM" src="https://github.com/user-attachments/assets/60c286b3-af22-444a-a2fa-4640a476b8b0" />

<img width="645" height="252" alt="Screenshot 2026-03-29 at 4 35 33 PM" src="https://github.com/user-attachments/assets/97fa5acc-e078-425d-ab21-1f99645e0e8d" />

<img width="570" height="619" alt="Screenshot 2026-03-29 at 4 37 27 PM" src="https://github.com/user-attachments/assets/ffa91775-78ac-4758-86d1-feeab96e1a1c" />

<img width="579" height="279" alt="Screenshot 2026-03-29 at 4 38 46 PM" src="https://github.com/user-attachments/assets/83101376-9140-4742-b042-0a61115fb2b6" />

<img width="577" height="184" alt="Screenshot 2026-03-29 at 4 39 33 PM" src="https://github.com/user-attachments/assets/01a4aba4-f9b2-4300-b583-596e1058a064" />

<img width="582" height="232" alt="Screenshot 2026-03-29 at 4 40 16 PM" src="https://github.com/user-attachments/assets/b0b42daa-87d4-4b98-abe9-cfcffe95c035" />

<img width="579" height="176" alt="Screenshot 2026-03-29 at 4 41 03 PM" src="https://github.com/user-attachments/assets/2af15d2d-3925-4a65-be83-49c53c6b6071" />

<img width="573" height="343" alt="Screenshot 2026-03-29 at 4 41 34 PM" src="https://github.com/user-attachments/assets/4a295e22-2bbe-489a-83cd-c2aff2481755" />

<img width="586" height="537" alt="Screenshot 2026-03-29 at 4 42 32 PM" src="https://github.com/user-attachments/assets/b5cd5644-81dc-42c7-9fdf-f6bf9e327223" />

<img width="576" height="349" alt="Screenshot 2026-03-29 at 4 43 39 PM" src="https://github.com/user-attachments/assets/eeb7b286-b6cb-4904-abfe-cf1d55964d8b" />

<img width="586" height="520" alt="Screenshot 2026-03-29 at 4 45 06 PM" src="https://github.com/user-attachments/assets/bf793499-fb0b-4238-b1ac-143d324e63b2" />

## Queries
<img width="563" height="271" alt="Screenshot 2026-03-29 at 9 57 11 PM" src="https://github.com/user-attachments/assets/d4197e84-5b21-401e-b6f6-0160a568fcec" />

### Query 1
<img width="551" height="384" alt="image" src="https://github.com/user-attachments/assets/a3ff4aa3-7d3f-4bfb-929d-834f3ed17a5e" />

Query 1 provides the user

### Query 2
<img width="576" height="346" alt="Screenshot 2026-03-29 at 10 01 34 PM" src="https://github.com/user-attachments/assets/b40fdcb2-5dfd-43b0-ae95-4f2738dc216d" />

Query 2 provides the user

### Query 3
<img width="576" height="347" alt="Screenshot 2026-03-29 at 10 02 04 PM" src="https://github.com/user-attachments/assets/d570f84f-057c-424c-a416-0934cf6dd79c" />

Query 3 provides the user


### Query 4
<img width="577" height="364" alt="Screenshot 2026-03-29 at 10 02 38 PM" src="https://github.com/user-attachments/assets/98881c9f-ffa0-46d4-8428-ab3cbf68f654" />

Query 4 provides the user

### Query 5
<img width="561" height="347" alt="Screenshot 2026-03-29 at 10 03 09 PM" src="https://github.com/user-attachments/assets/cafecc28-7e0b-433a-a5bf-3aa682018da4" />

Query 5 provides the user


### Query 6
<img width="582" height="332" alt="Screenshot 2026-03-29 at 10 03 43 PM" src="https://github.com/user-attachments/assets/adc3fecc-c1f9-48e3-a85b-ad7491ec9710" />

Query 6 provides the user


### Query 7
<img width="576" height="339" alt="Screenshot 2026-03-29 at 10 04 14 PM" src="https://github.com/user-attachments/assets/0ae61a8f-f2b2-4cd5-bcd1-d2c15e9545da" />

Query 7 provides the user


### Query 8
<img width="581" height="358" alt="Screenshot 2026-03-29 at 10 04 48 PM" src="https://github.com/user-attachments/assets/fc891563-0dd4-416f-b48b-f4b9320b8ed5" />

Query 8 provides the user

### Query 9
<img width="583" height="354" alt="Screenshot 2026-03-29 at 10 05 17 PM" src="https://github.com/user-attachments/assets/960f0b1d-058a-4163-87f9-c8f3a72c62a6" />

Query 9 provides the user


### Query 10
<img width="589" height="211" alt="Screenshot 2026-03-29 at 10 05 50 PM" src="https://github.com/user-attachments/assets/11e2d49a-82c5-48bc-a1a1-36459b0f2c0f" />

Query 10 provides the user














