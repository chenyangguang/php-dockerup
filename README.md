# php-dockerup
   A simple docker environment with nginx & php-fpm.
   
# Dir tree

`
├── docker-compose.yml
├── sme
└── sme.conf
`

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

  Check for the service running  with `docker-compose ps` command, or check for running  sth. with 
  `
  ➜  demo dp logs -f
Attaching to demo_php_1, demo_web_1
php_1  | [10-Apr-2018 13:07:18] NOTICE: fpm is running, pid 9
php_1  | [10-Apr-2018 13:07:18] NOTICE: ready to handle connections
php_1  | [10-Apr-2018 13:07:18] NOTICE: systemd monitor interval set to 10000ms
`.
  
# Short command with docker-compose

  Add `echo  'alias dp="docker-compose"'  >> ~/.zshrc` (~/.zshrc or ~/.bashrc) to the last line in any of yourself shell config file. Then `source ~/.zshrc` , So we can use *dp* command short for *docker-compose*.
  
