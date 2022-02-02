# Selenium_Grid_Docker_Compose
Assignment : Selenium Hub/Grid on Docker Compose

Open Terminal on your local machine where docker-compose.yml is
Then
Run Docker Compose file
To run the Docker Compose file, simply run the following command on the terminal  "docker-compose up"


Setup Parallel Execution with Docker Compose
There are 2 ways to set up parallel execution for Selenium Grid using Docker Compose -

Updating Docker Compose file: Add NODE_MAX_INSTANCES and NODE_MAX_SESSION to the Docker services 

Dynamically increasing the nodes: using Docker scale command, you can also dynamically add more nodes  " docker-compose up --scale firefox=3" this will add total 3 nodes for Firefox

using this 
http://172.20.0.2:4444/grid/cosole   #this url you will find in log after you hit "docker-compose up" 

on your browser you can see number of browsers
that mean this machine can be use to run this number of browsers parallelly

as we see in above commands we can change numbers of instances using docker-compose as well as dynamically on Command Line
