# Rasa is for everyone
This is a german RASA3 Starter Pack with use of docker.
Follow this readme to get it up and running.

Have Fun!
:-) 



# Howto
## 1 Build a dockerimage with name rasa3docker
docker build -t rasa3docker .

## 2. Run and use the image

### 1. buld container (firsttime run)
docker run --name rasa3docker -v "${pwd}:/opt/mybot" -w "/opt/mybot" -it rasa3docker bash
### 2. start container (if Step 1. happend already and container is closed)
docker start myRasabot   
### 3. get into already startet container
docker exec -it myRasabot bash

## 4. use rasa into container
* rasa train 
* rasa shell
* rasa run actions --actions actions --debug --auto-reload

## 3. Starter Tutorials

Tutorial: https://www.youtube.com/watch?v=sazsWmP2d3o

Source: https://github.com/RasaHQ/pokedex-demo

Rasa Youtube Channel in General. Have an eye on the rasa versions. 

## 4. Current bot usage

Just say "hallo" and chat. 
