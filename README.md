# PHP dockerup

   A simple docker environment with nginx & php-fpm & mysql.
   
# Depends 

  * [docker install](https://docs.docker.com/install/#supported-platforms)
  
  * [docker-compose install](https://github.com/chenyangguang/php-dockerup/edit/master/README.md)
  
# Install

`
  git clone https://github.com/chenyangguang/php-dockerup.git 
`
  
# Up and down work

  - `docker-compose up -d `
  
  - `docker-compose ps`
  
  - `docker-compose down -d`
  
# Short command with docker-compose

  Add 
  
  `
    echo  'alias dp="docker-compose"'  >> ~/.zshrc
  ` 
  
  (~/.zshrc or ~/.bashrc) to the last line in any of your shell config file. Then operation 
  

  `
  source ~/.zshrc 
  `
  
   So we can use ***dp*** command short for ****docker-compose***.
  
