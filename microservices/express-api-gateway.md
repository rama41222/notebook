### Express based api Gateway

##### Overview

* To learn how an API gateway by building from scratch
* To integrate with microservices and api rate limiting functionality via REDIS

##### Research 

* Based on the initial research, this gateway will have a set of hardcoded routes as required by the microservices.
* Basic routing example. For more, refer [express-routing](https://expressjs.com/en/guide/routing.html)
```
routes.get('/regex/', ()=>{});
``` 
* Later on routes will be generated from the data taken from a .yml file for easier configuration.
* Main **disadvantage** of express based api-gateway is it's single threaded. So sometimes building an api gateway 
out of exressjs might not be the case.
 
