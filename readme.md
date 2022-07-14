# Rasa is for everyone
This is a german RASA3 Starter Pack with use of docker.
Follow this readme to get it up and running.

Have Fun!
:-) 

# Howto
### Build a dockerimage with name rasavoicedocker
docker build -t rasa3docker .

## 2. Run and use the image

### buld container
docker run --name rasa3docker -v "${pwd}:/opt/mybot" -w "/opt/mybot" -it rasa3docker bash
### start container
docker start myRasabot   
### get into already startet container
docker exec -it myRasabot bash

## use rasa into container
rasa train 
rasa shell
rasa run actions --actions actions --debug --auto-reload


## Best Starter Tutorial (I found)
https://github.com/RasaHQ/pokedex-demo
https://www.youtube.com/watch?v=sazsWmP2d3o
