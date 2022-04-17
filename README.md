# Docker Build Command
  Docker build .

#   Docker Build Command
    docker build -t chakradharijena545/webapplication .

#   Docker Connecting port from local system to docker container
    docker run -p 8080:8080 chakradharijena545/webapplication

#   Docker to open Shell
    docker run -it chakradharijena545/webapplication sh

#   Docker to open Shell
#   How to open a shell inside docker and check the file location also?
Ans:-
PS D:\Docker\webapplication> docker run -p 8080:8080 chakradharijena545/webapplication
Listening port 8080

PS D:\Docker\webapplication> docker ps
CONTAINER ID   IMAGE                               COMMAND                  CREATED          STATUS    
      PORTS                    NAMES
8ab3ffaaddb0   chakradharijena545/webapplication   "docker-entrypoint.s…"   11 seconds ago   Up 10 seconds   0.0.0.0:8080->8080/tcp   nifty_kilby
PS D:\Docker\webapplication> docker exec -it 8ab3ffaaddb0 sh  