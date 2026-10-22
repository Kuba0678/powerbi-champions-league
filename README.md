# UEFA Champions League 2024/2025 - Power BI Dashboard 

An interactive Power BI dashboard showing comprehensive team and player statistics for the 2024/2025 UEFA Champions League (the first season using the new Swiss-system format). 

I built this project in collaboration with Jakub Klim. Together, we handled everything from gathering the raw data to creating the final interactive visuals.

## Project Overview
* **Data Preparation (ETL):** We extracted data from FBREF and TransferMarkt and cleaned it using Power Query. We worked with 16 different tables, fixing data types, standardizing names, and creating lookup tables.
  
* **Data Modeling:** We connected the tables using a Snowflake schema, organizing them into 2 dimension tables (Teams, Players) and 14 fact tables.
  
* **DAX Formulas:** We wrote custom DAX measures to calculate different stats. We also used Field Parameters and the `CALCULATE` function so the charts update automatically when a user selects different filters.
  
* **Design & Interactivity:** We created 3 clean, dark-themed dashboard pages (Team's, Player's, and Goalkeeper's Stats). We added a "Drill Through" feature to explore specific club details, and used the `SELECTEDVALUE` function to make team logos and stadium photos render dynamically based on the selected team.

## Dashboard Previews

### 1. Main Dashboard - Teams Overview
<img width="655" height="368" alt="1" src="https://github.com/user-attachments/assets/6967e28c-7df9-4bcb-af2c-c440fe8a9149" />
### Main Dashboard - Team Filter applied
<img width="654" height="368" alt="2" src="https://github.com/user-attachments/assets/f226f559-8cf4-4318-ac7b-32119571f681" />


*Overview of all teams participating in the tournament.*

### 2. Player's Stats - Squad Overview
<img width="636" height="359" alt="3" src="https://github.com/user-attachments/assets/b3a79355-b5f0-479a-8b04-8280d43d8ffb" />

### Player's Stats - Individual Profile
<img width="638" height="360" alt="4" src="https://github.com/user-attachments/assets/ece4f87b-1064-4d72-9dbb-0aa4a2cbc139" />

### Goalkeepers - League Comparison
<img width="640" height="362" alt="5" src="https://github.com/user-attachments/assets/fc77b336-8d02-4ce9-8f8f-b8ce06027028" />

### Goalkeepers - Specific Player Filter
<img width="637" height="361" alt="6" src="https://github.com/user-attachments/assets/47a45a81-9c48-4420-b579-8183c0b9a65f" />


*Detailed player statistics featuring custom radar charts.*

### 3. Drill Through - Club Deep Dive
<img width="641" height="360" alt="7" src="https://github.com/user-attachments/assets/0636eb53-de36-4b2d-ae4b-1fc2cdf4835d" />


*Specific club view showcasing dynamic loading of the stadium photo and club logo.*

## How to view the project
1. Download the `.pbix` file from this repository.
2. Open it using Microsoft Power BI Desktop.
3. Use the filters on the left panel or right-click on a specific team/player to use the "Drill Through" feature.
