# CRUD  
This is a simple CRUD application. This monorepo contains an API and a frontend APP . Each
directory has a simple Dockerfile . 
 
# Requirenments 
1. docker
2. docker-compose
 
# How to Run This Application? 
After complete all requirements, you just run the below commands.

> docker-compose build<br> Firstly build 
> docker-compose up<br> Run all service in docker-compose file
> docker-compose run api rails db:create<br> initialize database
> docker-compose run api rails db:migrate db:seed<br> load database schemas

# Result

You can view Rails welcome page on http://localhost:3000. This app should now be running on port 3000 on your Docker daemon.
