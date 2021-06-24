# Test for Confiax

#### This a simple project with an api and client to list, show and create users in a mysql database



## Used Techs
### Infrastructure
- Docker
- Mysql database

### Api
- NestJS
- TypeORM

### Client
- ReactJS

## To run this project
Make sure that Docker is installed on your server or local machine.

This project uses the git submodule feature. But don't worry, if you're not familiar with submodules, you'll still be able to run and test the project

### Step by step
- Clone this repository and submodules
```git 
    git clone --recurse-submodules https://github.com/ClaitonBarreto/confiax.git
```

- Run only the ```mysql``` container (this is necessary because typeORM can't create database directly).


```docker 
    docker-compose up mysql -d
```

- Access the database through your preferred database managment system

- Create a databse with name ```confiax```

- Run the others services

- If you only run the project, run docker-compose command in root directory

```docker 
    docker-compose up -d
```

- After few minutes (docker will go download base images and create containers) you can access http://localhost:3000 in your browser, and use the application
