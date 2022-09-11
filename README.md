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

![Bootstrap5 2 0](https://user-images.githubusercontent.com/113204580/189523622-f7a4cc09-1d89-4a8c-8c8c-968f3907bc8a.png)

## Common commands ###

#### to create the database ####
    
    docker-compose run web rake db:create

### generate controller ###

    docker-compose exec web rails g controller home index

### rails console ####

    docker-compose exec web rails console
or

    docker-compose run web rails console
