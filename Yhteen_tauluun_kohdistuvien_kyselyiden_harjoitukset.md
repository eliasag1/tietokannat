# Yhteen tauluun kohdistuvien kyselyiden harjoitukset 

### Tehtävä 1
select * from goal

<img width="784" alt="yhteentauluun1" src="https://github.com/user-attachments/assets/fcdb5c32-0430-45a3-ab91-6ca4326fb4a1">


### Tehtävä 2
select name airport_type from airport where iso_country = "FI";
<img width="657" alt="yhteentaluun2" src="https://github.com/user-attachments/assets/92ba96ad-1c69-450a-8973-2f1cac4528f5">

### Tehtävä 3
select name from airport where iso_country = "FI" order by name;
<img width="950" alt="yhteentauluun3" src="https://github.com/user-attachments/assets/82b27779-e160-4922-baad-eab4aa799245">

### Tehtävä 4
select name, type from airport where iso_country = "FI" order by type, name;
<img width="704" alt="Näyttökuva 2024-09-16 kello 13 37 19" src="https://github.com/user-attachments/assets/6e44f676-63e4-41db-95ee-b38f3c9a1b16">


### Tehtävä 5
select name from country where name like "F%";

<img width="492" alt="Näyttökuva 2024-09-16 kello 13 46 18" src="https://github.com/user-attachments/assets/87a61396-3865-4e3c-947e-d33279205cdf">

### Tehtävä 6
select name from country where name %F%";

<img width="500" alt="Näyttökuva 2024-09-16 kello 13 48 15" src="https://github.com/user-attachments/assets/c267ed40-bb1e-4b9f-b481-ddc77e4cab2f">

### Tehtävä 7
select location from game where screen_name = "Vesa";

<img width="542" alt="Näyttökuva 2024-09-16 kello 13 53 05" src="https://github.com/user-attachments/assets/8bee5627-71dc-40e8-bde6-5fc800a96339">

### Tehtävä 8
select co2_consumed from game where screen_name = "Ilkka";

<img width="578" alt="Näyttökuva 2024-09-16 kello 13 54 05" src="https://github.com/user-attachments/assets/76281aea-ab7b-457b-846f-75817bb463e5">

### Tehtävä 9
select distinct co2_budget from game;

<img width="427" alt="Näyttökuva 2024-09-16 kello 13 54 53" src="https://github.com/user-attachments/assets/b4021740-5fd4-47c9-98d4-130f414ee139">


