# CRUD  
This is a simple CRUD application. This monorepo contains an API and a frontend APP . Each
directory has a simple Dockerfile . 
 
# Requirenments 
1. docker
2. docker-compose
 
# How to Run This Application? 
After complete all requirements, you just run the below commands.


> $docker-compose build<br>
> $docker-compose up<br> 
> $docker-compose run api rails db:create<br> 
> $docker-compose run api rails db:migrate db:seed<br>

# Result

You can view Rails welcome page on http://localhost:3000. This app should now be running on port 3000 on your Docker daemon.