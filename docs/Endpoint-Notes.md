The `/notes` endpoint requires a single argument of claim number. It returns note data based on the claim number provided.
```
/notes/<claim_num>.json
```
### Example
```
/notes/012345.json
```
### Fields
The following fields are returned for each row in the result set.
* claim_number
* note_text
* note_user
* utc_note_date
