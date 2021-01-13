# NodeJs-Redis-caching-routes

Redis + Node.js project showing how to use caching services in a single route.
Where that route is responsible for getting the number of repos for the given github username using Github APIs.
The server will check if the username exists first in the redis db using a middleware function, then respond with the number of repos, also the cached data are given a Time To Live value of 1 hour to make sure the data is always fresh.
