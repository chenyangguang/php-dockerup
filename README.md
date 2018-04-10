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

  `docker-compose up -d `
  
If every thing works well, it will turn out like below:  
  
  `➜  demo dp up -d
  
   Creating network "demo_sme-network" with driver "bridge"

   Creating demo_web_1 ... done

   Creating demo_php_1 ... done`


Shutdown the service and kill will connect docker ps the this project with: 
  
  `docker-compose down -d`
  
  `➜  demo dp down  
  
  Stopping demo_php_1 ... done

  Stopping demo_web_1 ... done

  Removing demo_php_1 ... done

  Removing demo_web_1 ... done

  Removing network demo_sme-network`

Check for the service running  with
  
  `docker-compose ps`
  
# Short command with docker-compose

  Add 
  
      `echo  'alias dp="docker-compose"'  >> ~/.zshrc` 
  
  (~/.zshrc or ~/.bashrc) to the last line in any of yourself shell config file. Then 
  
      `source ~/.zshrc` 
  
   So we can use *dp* command short for *docker-compose*.
  
