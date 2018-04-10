# php-dockerup
   A simple docker environment with nginx & php-fpm.
   
# Depends 
  * [docker install](https://docs.docker.com/install/#supported-platforms)
  
  * [docker-compose install](https://github.com/chenyangguang/php-dockerup/edit/master/README.md)
  
# Install

  <pre><code>
  git clone https://github.com/chenyangguang/php-dockerup.git 
  </code></pre>
  
# Up and down work

  - `docker-compose up -d `
  
  - `docker-compose ps`
  
  - `docker-compose down -d`
  
# Short command with docker-compose

  Add 
  
      `echo  'alias dp="docker-compose"'  >> ~/.zshrc` 
  
  (~/.zshrc or ~/.bashrc) to the last line in any of yourself shell config file. Then 
  
      `source ~/.zshrc` 
  
   So we can use *dp* command short for *docker-compose*.
  
