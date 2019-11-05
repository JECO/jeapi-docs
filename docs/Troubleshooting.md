If you're continuously getting errors, check the status of the server to ensure it is up. 
To quote the wiki on the `/status` endpoint:

> The `/status` endpoint is useful for troubleshooting whether or not the server is down or credentials are bad, as in some cases the server may provided a generic error when credentials are bad or a token is expired.

> __Simply checking server status does not require authentication__ (and is the only endpoint that does not).

> To check status, send the below cURL request.
> ```
> curl -X GET https://je-api.com/v0/status.json
> ```
> If the server is up, you'll receive the following message:
> ```
> {"message": ["JEAPI is up."]}
> ```
> You can also simply navigate to this endpoint ([click here](https://je-api.com/)) in your browser to see if the server is up.

If the server is up, do the following:
1. Make sure that your credentials are entered in properly. 
2. Ensure you're using the JWT before it expires (see the [authentication page](https://github.com/JECO/jeapi-docs/wiki/Authentication) for more information on JWT expiration).
3. Ensure your syntax is correct (if you're sending cURL commands from Windows, you'll need to escape certain characters or payloads).

If you've followed the steps above, your credentials may be invalid and you should contact the [Johns Eastern Helpdesk](https://je.zendesk.com/hc/en-us/requests/new) for assistance.