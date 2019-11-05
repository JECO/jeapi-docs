### Format
Responses always return as JSON files keyed with one of three keys:
* Results - This indicates that results were found for the requested call, the value will generally be a list of JSON dictionaries.
* Message - This key holds a message from the server that is not a server error. Most often this means no results were found.
* Error - Indicative of an error, either server or client side. The value will inform you of more specific details.

The value of the key will always be a list, and will often be a list of JSON dictionaries.

### Examples
```
{"results": ["012345", "012346", "012347", ...]}
```
```
{'message' = ['No results found.'])}
```
```
{'error' = ['Failed to authenticate, AIM token not issued correctly.']}
```
