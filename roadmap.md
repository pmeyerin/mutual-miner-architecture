#Roadmap

##0.1.0 goals

###Click websocket exists
Should be unsecured
Accepts int representing number of clicks since last update
responds with int representing total number of clicks
With the total being the previous total, as saved to the database, plus the click count in the request body

###Basic UI exists
Client should be ReactJS
Should track a local click count
Should periodically update the count with the service and use the response to confirm the local count

###Basic database exists
Requires only one table `PlayerState`
```
playerId    -   string
clickCount  -   long
```