The `/status` endpoint is useful for troubleshooting whether or not the server is down or credentials are bad, as in some cases the server may provided a generic error when credentials are bad or a token is expired.

__Simply checking server status does not require authentication__ (and is the only endpoint that does not).

To check status, send the below cURL request.
```
curl -X GET https://je-api.com/v1/status.json
```
If the server is up, you'll receive a success message.
```
{"message": ["<Message varies by version.>"]}
```
You can also simply navigate to this endpoint ([click here](https://je-api.com/)) in your browser to see if the server is up.
See the [troubleshooting page](https://github.com/JECO/jeapi-docs/wiki/Troubleshooting) for further help.
