### Information
The JE API uses [JWT (JSON Web Token)](https://en.wikipedia.org/wiki/JSON_Web_Token) authentication to verify your identity and to help retrieve relevant information to your organisation. 
<br><br/>
To make a call to the API, you'll need your API token username and password supplied by Johns Eastern (not to be confused with the JSON web token that the server will generate). If you do not have this, please contact the [Johns Eastern Helpdesk](https://je.zendesk.com/hc/en-us/requests/new).
<br><br/>
You'll send the request to the `/auth` endpoint of the API, however, it is important to note that this endpoint does not append to the version number of the API. Meaning that __no matter the version, the authentication endpoint will always be `https://je-api.com/auth`.__
### Obtaining the JWT
To obtain the webtoken, send your credentials in a cURL request to the server `/auth` endpoint.
* Unix:
  ```
  curl -H "Content-Type: application/json" -X POST -d "{"username":"0123456789","password":"0123456789876543210"}" https://je-api.com/auth
  ```
* Windows:
  ```
  curl -H "Content-Type: application/json" -X POST -d "{\"username\":\"0123456789\",\"password\":\"0123456789876543210\"}" https://je-api.com/auth
  ```

If all goes well, you should receive a lengthy JSON response like the following format:
```
{"access_token":"qwertyuiopasdfghjklzxc.asdfghjklzxcvbnmqwertyuiop.zxcvbnmqwertyuiopasdfghjklzxcvbnm-QW"}
```
### Expiration 
JWTs expire within 5 minutes. It is best practice to request a new token with each call to ensure your request isn't rejected due to an expired token.

<br><br/>
If you have any issues with authentication, see the [troubleshooting wiki page](https://github.com/JECO/jeapi-docs/wiki/Troubleshooting).