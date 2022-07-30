# Commands

Example 1: 

a) Clone the repo using below command:

# git clone https://github.com/nics90/docker-session.git

b) Navigate to example1 directory:

# cd docker-session/docker_file/example1

c) Create a custom image with apache2 and custom page index.html

# docker build -t webapp1 .

d) Spin up the container to run webapp 

# docker run -d -p 8080:80 webapp1

e) Go to browser and access the website at url - http://hostIP:8080


Example 2:

a) Navigate to example2 directory:

# cd docker-session/docker_file/example2

b) Create a custom image with figlet installed:

# docker build -t figletapp1 .

c) Run the container without any argument to see the banner:

# docker run figletapp1

Output:
 _          _   _
| |        | | | |
| |     _  | | | |  __
|/ \   |/  |/  |/  /  \_
|   |_/|__/|__/|__/\__/

d) Now pass an argument to overwite CMD content:

# docker run figletapp1 DevOps

Output:

  ____             __
 (|   \           /\_\/
  |    | _       |    |  _   ,
 _|    ||/  |  |_|    ||/ \_/ \_
(/\___/ |__/ \/   \__/ |__/  \/
                      /|
                      \|

Example 3 : 

a) Navigate to example3 directory:

# cd docker-session/docker_file/example3

b) Create a custom image to host flask application:

# docker build -t flaskapp1 .

c) Spin up the container to run flask application:

# docker run -d -p 5000:5000 flaskapp1

d) Go to browser and access the app at url - http://hostIP:5000 & http://hostIP:5000/devops

Example 4 : Docker Compose Installation 

a) Navigate to below directory :

# cd docker-session/docker_compose

b) Run the script install_compose.sh to install docker compose:

# sh install_compose.sh

Example 5 : Install Wordpress using docker compose :

a) Navigate to directory :

# cd docker-session/docker_compose/example1

b) Run the below command :

# docker-compose up -d

c) Access the wordpress at url : http://hostIP:8000

d) To clean up :

# docker-compose down






