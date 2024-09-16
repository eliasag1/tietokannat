# Where-osan liitosehto harjoitukset

### Tehtävä 1
select country.name as "country name", airport.name as "airport name"
from airport, country
where airport.iso_country = country.iso_country and country.name = "Iceland";

<img width="651" alt="Näyttökuva 2024-09-16 kello 13 59 55" src="https://github.com/user-attachments/assets/39877bbf-99d2-4169-b6dc-ceebb857cd4f">

### Tehtävä 2

select airport.name as "airport name"
from airport, country
where airport.iso_country = country.iso_country and country.name = "France" and airport.type = "large_airport";

<img width="838" alt="Näyttökuva 2024-09-16 kello 14 07 53" src="https://github.com/user-attachments/assets/9ab27209-3b69-4c69-bc29-0319a1f0ba13">

### Tehtävä 3

select country.name as country_name, airport.name as airport_name
from airport, country
where airport.iso_country = country.iso_country and country.continent = "AN";

<img width="624" alt="Näyttökuva 2024-09-16 kello 14 42 44" src="https://github.com/user-attachments/assets/bc9d9fe1-8b6d-44b5-b853-ade7e507010a">

### Tehtävä 4

select elevation_ft
from airport, game
where location = ident and screen_name = "Heini";

<img width="403" alt="Näyttökuva 2024-09-16 kello 14 44 14" src="https://github.com/user-attachments/assets/6cb269a8-e76e-497e-bd8e-5c77548c6436">

### Tehtävä 5

select elevation_ft * 0.3048 as elevation_m
from airport, game
where location = ident and screen_name = "Heini";

<img width="466" alt="Näyttökuva 2024-09-16 kello 14 45 12" src="https://github.com/user-attachments/assets/72b3fab7-4814-4a57-b947-e02038b53877">

### Tehtävä 6

select name
from airport, game
where location = ident and screen_name = "Ilkka";

<img width="404" alt="Näyttökuva 2024-09-16 kello 14 47 01" src="https://github.com/user-attachments/assets/c2a432db-b284-4273-a35c-880240e92b97">

### Tehtävä 7

select country.name
from airport, game, country
where location = ident and airport.iso_country = country.iso_country  and screen_name = "Ilkka";

<img width="728" alt="Näyttökuva 2024-09-16 kello 14 48 31" src="https://github.com/user-attachments/assets/355e6b8d-eaf4-49b6-bf56-8bfd0a6eaed6">

### Tehtävä 8

select name
from goal, goal_reached, game
where game.id = game_id and goal.id = goal_id and screen_name = "Heini";

<img width="558" alt="Näyttökuva 2024-09-16 kello 14 49 31" src="https://github.com/user-attachments/assets/b89c56a9-14bf-462c-a11e-833028677208">

### Tehtävä 9
	
select airport.name
from airport, game, goal, goal_reached
where ident = location and game.id = game_id and goal.id = goal_id and screen_name = "Ilkka" and goal.name = "CLOUDS";

<img width="881" alt="Näyttökuva 2024-09-16 kello 14 50 30" src="https://github.com/user-attachments/assets/ddb99065-619f-40b3-b5d1-37f9a0155e48">

### Tehtävä 10 

select country.name
from country, airport, game, goal, goal_reached
where airport.iso_country = country.iso_country and ident = location and game.id = game_id and goal.id = goal_id and screen_name = "Ilkka" and goal.name = "CLOUDS";

<img width="1020" alt="Näyttökuva 2024-09-16 kello 14 51 24" src="https://github.com/user-attachments/assets/be7b5edc-e69c-4a9a-9c06-bd8a2b12b57c">



