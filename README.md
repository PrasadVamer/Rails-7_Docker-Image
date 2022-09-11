# Rails 7 on Docker

This sets up a Ruby on Rails ~>7.0.4 app using Docker and Docker-Compose to pull in docker images of Ruby 3.1.2 and Postgres 14.5

## Clone The repository ##

    git clone https://github.com/PrasadVamer/Rails-7_Docker-Image.git
    
## Start the container ##  

Start the container (while building) by running the following command:

    docker-compose up --build
    
## View the page in your browser ##

Now, let's access http://localhost:3000/ and check if Rails is working properly.

## You are good to go ##
You will get the following web page.

![Rails7 0 4](https://user-images.githubusercontent.com/98350622/189521802-74d8a5a5-946b-417e-86ce-bc52fe091a16.png)

## Common commands ###

#### to create the database ####
    
    docker-compose run web rake db:create
### rails console ####

    docker-compose exec web rails console
or

    docker-compose run web rails console
