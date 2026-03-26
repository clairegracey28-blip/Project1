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

<img width="589" height="745" alt="Screenshot 2026-03-26 at 8 24 23 AM" src="https://github.com/user-attachments/assets/bffdb22b-9594-492e-be86-7f5285550e4d" />
