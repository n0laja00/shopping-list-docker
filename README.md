# shopping-list-app

Author: n0laja00

I'm using javascript with eta, a javascript template engine. Visit eta's official site at: https://eta.js.org/ if you're interested!

This app uses elephant SQL with a connection pool of concurrent connections of 2.

This project uses docker (Docker desktop)! To read more about docker, visit: https://www.docker.com/. To get Docker Desktop, visit: https://docs.docker.com/desktop/install/windows-install/

I expect you to have Docker installed, as this isn't a guide on how to install Docker.

What is needed to launch this project? 
 - docker
 - (Free) port: 7777

Database information is outlined in .project.env -file. 
![image](https://user-images.githubusercontent.com/73889850/192112125-7c45127d-c340-4ebb-b981-b8f36b1a034f.png)

and they are used in a variety of locations, but this is the most important. 

```./app/database/database.js``` has the following code:
![image](https://user-images.githubusercontent.com/73889850/192112158-ccbe2a4a-4060-4b7d-bae0-08530d5815d3.png)

The database exists on port: ```5432```. 


## How to launch the project? 

In the root folder, the folder that has **docker-compose.yml, project.env, and this README.md**, run the following command: ```docker-compose up```

![image](https://user-images.githubusercontent.com/73889850/192112258-d7708b7b-1ac3-4848-8f78-9883f41c6480.png)

When successfull, you'll see the following:

![image](https://user-images.githubusercontent.com/73889850/192112299-3eb8afa0-6fb5-4199-a671-b918a3d288d9.png)

And can access localhost:7777 to see: 

![image](https://user-images.githubusercontent.com/73889850/192142816-aeaf2edc-93ed-4351-a42b-2beacdb385b8.png)

To see the application in action, visit Heroku at: https://n0laja00-shopping-list-app.herokuapp.com/
