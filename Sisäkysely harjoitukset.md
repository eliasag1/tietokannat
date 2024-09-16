# Sisäkysely harjoitukset

### Tehtävä 1

select name
from country
where iso_country in(
select iso_country
from airport
where name like "Satsuma%"
);

<img width="254" alt="Näyttökuva 2024-09-16 kello 15 04 00" src="https://github.com/user-attachments/assets/e526d4e2-acac-4fcb-b25f-01d6063f48fc">

### Tehtävä 2

select name
from airport where
iso_country in(
select iso_country
from country
where name = "Monaco"
);

<img width="264" alt="Näyttökuva 2024-09-16 kello 15 04 45" src="https://github.com/user-attachments/assets/4896aab1-6b62-44fb-928c-c134d7a22bb3">

### Tehtävä 3

select screen_name
from game
where id in (
select game_id
from goal_reached
where goal_id in(
select id
from goal
where name = "CLOUDS"
)
);

<img width="127" alt="Näyttökuva 2024-09-16 kello 15 05 35" src="https://github.com/user-attachments/assets/392241c3-46da-46ea-9eb8-a02d27d7b82f">

### Tehtävä 4

select country.name
from country
where iso_country not in
(select airport.iso_country
from airport);

<img width="238" alt="Näyttökuva 2024-09-16 kello 15 06 47" src="https://github.com/user-attachments/assets/662a51c0-575d-4414-b49b-66d0ce968e31">

### Tehtävä 5

select name
from goal
where id not in(
select goal.id
from goal, goal_reached, game
where game.id = game_id and goal.id = goal_id and screen_name = "Heini"
);

<img width="72" alt="Näyttökuva 2024-09-16 kello 15 07 29" src="https://github.com/user-attachments/assets/a184802d-7e65-4b6d-802b-0309bf51d4a9">

