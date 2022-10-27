# Docker Laravel App
In this project, here i implement laravel with docker in the local environment using the LEMP stack that includes: Nginx, MySQL, PHP, and phpMyAdmin.
 
## How to Install and Run the Project

Step-1. ```git clone https://github.com/mamunurrashid1010/Docker-Laravel-App.git```<br>
Step-2. Go to project src directory ```cd src```<br>
Step-3. ```composer install```<br>
Step-4. Copy ```.env.example``` to ```.env``` <br>
Step-5. Open ``` .env ``` file and update
```
DB_CONNECTION=mysql
DB_HOST=db
DB_PORT=3306
DB_DATABASE=blog
DB_USERNAME=root
DB_PASSWORD=password
```
Step-6. ```docker-compose build``` <br>
Step-7. ```docker compose up -d``` <br>
You can see the project on ```http://127.0.0.1:8080``` <br>
Open ```phpMyAdmin``` on ```127.0.0.1:3400```

## How to run Laravel Commands with Docker Compose
1. Go to project src directory ```cd src```<br>
2. Command ```docker-compose exec app php artisan {your command}``` <br>