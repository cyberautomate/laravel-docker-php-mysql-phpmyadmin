## This is Laravel ready Docker container

## Contents
- Laravel 9
- Composer 2.4
- Apache
- PHP 8.1
- MySQL 8
- PHPMyAdmin

## Build / usage instruction

1. To build the container you will first need [docker desktop](https://www.docker.com/products/docker-desktop/) installed. I did this all on a Windows host but the process should be similar on MAC/Linux.

2. Clone the repository to a folder on the client. For the sake of clarity let's say we cloned the repo to c:\ which would result in a folder called c:\laravel-docker-php-mysql-phpmyadmin. You can change this to whatever yopu want.

The folder structure should look like this. The only files/folders here that are not part of the typical Laravel file structure are noted in the image below. All of the docker build specific configuations most reside in the **dockerfile** and the **docker-compose.yml**
![image](https://user-images.githubusercontent.com/95773446/210823628-4f7565c3-53a7-4b1c-a467-e997f46eeb88.png)

3. Build the images and run the container
    - In Windows Terminal navigate to the folder where you downloaded everything and run ```docker-compose up --build```
    - Once complete you should see some output in the terminal simialr to the image below.
 ![image](https://user-images.githubusercontent.com/95773446/210824990-a6839371-fbad-44d5-8170-4e499cdcd1d2.png)

4. Confirm the images are built and the containers are running in Docker Desktop, see the example images below

![image](https://user-images.githubusercontent.com/95773446/210825334-222bc213-389d-4ae9-9781-083b0fb081b8.png)

![image](https://user-images.githubusercontent.com/95773446/210825457-d523a2dc-4c05-4e91-98bf-66c15ca377c5.png)

5. Everything should be good to go now. You can access the baseline Laravel application via http://localhost:8080

![image](https://user-images.githubusercontent.com/95773446/210825993-b3c58b9a-181c-4411-8f17-307738959e5b.png)

6. Access PHPmyAdmin to manage the Database here http://localhost:8001. Username and password are both ***root***

![image](https://user-images.githubusercontent.com/95773446/210826386-c64c5017-5e02-434b-bfee-1918e5c0a2cf.png)

&. Go build something cool. :)




