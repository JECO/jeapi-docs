To call the API, you'll pass a cURL request to a specific [endpoint](https://github.com/JECO/jeapi-docs/wiki/Endpoints) with the method and [JWT you received from the server](https://github.com/JECO/jeapi-docs/wiki/Authentication).
### Example
Below we will append the JWT to the end of a request to list all claim numbers. The `{URI}` below should be replaced with the relevant URI listed at the [current URI page](https://github.com/JECO/jeapi-docs/wiki/Current-URI).
```
curl -X GET {URI}/claims/view_all.json -H "Authorization: JWT qwertyuiopasdfghjklzxc.asdfghjklzxcvbnmqwertyuiop.zxcvbnmqwertyuiopasdfghjklzxcvbnm-QW"
```