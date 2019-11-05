The `/checks` endpoint requires at least one argument but takes up to three. It returns check data based on the arguments provided.
```
/checks/<from_date>/<to_date>/<claim_num>.json
```
To leave a field "blank", enter values like below:
* from_date = false
* to_date = false
* claim_num = all
```
/checks/false/false/all.json
```
However, you may run this example above and find the server responds with an error:
```
{"error": ["At least one keyword argument is required."]}
```
So you'll need to provide at least one non-default argument. See examples for more.
### Dates
All dates must be in format `YYYYMMDD`. Additionally, dates and times are in UTC format and are returned as [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) strings.
### Examples
```
/checks/false/false/012345.json
```
Getting all checks after a date.
```
/checks/20190101/false/all.json
```
Getting all checks for a claim between two dates.
```
/checks/20190101/20170615/012345.json
```
### Fields
The following fields are returned for each row in the result set.
* check_amount
* check_num
* check_type
* fh_claim_num
* party
* payable_comment
* payee_name
* payment_type_name
* utc_check_date
* utc_void_date
* void_amount
* voided_yn
* check_amount
* check_num
* check_type
* fh_claim_num
* party
* payable_comment
* payee_name
* payment_type_name
* utc_check_date
* utc_void_date
* void_amount
* voided_yn
