# docker-session

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


