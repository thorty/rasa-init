Tutorial Source: https://github.com/RasaHQ/pokedex-demo
https://www.youtube.com/watch?v=sazsWmP2d3o

next step use slots to store info: 
1. ask if user wants mor info about choosen pokemon
2. ask which info
3. fetch and play info
https://www.google.com/search?client=firefox-b-d&q=use+slots+in+rasa#kpvalbx=_2MwGYrehOdbi7_UP2pmq2AU17

-- what if user asks other questions?...

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
https://dev.to/petr7555/series/11401
Rasa YouTube Channel




