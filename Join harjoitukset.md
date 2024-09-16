# Join harjoitukset

### Tehtävä 1

select country.name as "country name", airport.name as "airport name"
from country inner join airport on airport.iso_country = country.iso_country
where country.name = "Finland" and scheduled_service = "yes";

<img width="651" alt="Näyttökuva 2024-09-16 kello 14 55 24" src="https://github.com/user-attachments/assets/b6fd88b4-527f-48d2-b3df-57441f10d442">

### Tehtävä 2

select screen_name, airport.name
from game inner join airport on location = ident;

<img width="401" alt="Näyttökuva 2024-09-16 kello 14 56 17" src="https://github.com/user-attachments/assets/a58044a9-826c-465b-91f0-745d2b05b03b">

### Tehtävä 3

select screen_name, country.name
from game inner join airport on location = ident inner join country on airport.iso_country = country.iso_country;

<img width="848" alt="Näyttökuva 2024-09-16 kello 14 57 22" src="https://github.com/user-attachments/assets/f0f664be-496c-4dd4-8e21-872e29df001b">

### Tehtävä 4

select airport.name, screen_name
from airport left join game on ident = location where name like "%Hels%";

<img width="565" alt="Näyttökuva 2024-09-16 kello 14 58 28" src="https://github.com/user-attachments/assets/d2fe9594-b06a-413c-8bbc-54aa07803183">

### Tehtävä 5

select name, screen_name
from goal left join goal_reached on goal.id = goal_id  left join game on game.id = game_id;

<img width="689" alt="Näyttökuva 2024-09-16 kello 14 59 23" src="https://github.com/user-attachments/assets/ce52f5f5-204c-464f-b3cf-638d9edf751f">




