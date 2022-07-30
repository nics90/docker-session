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
