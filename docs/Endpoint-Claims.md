The `/claims` endpoint can be used to return detail on claims or a list of claims.
### Usage
This returns a list of all claims you have access to.
```
/claims/view_all.json
```
You can pass a claim number to get specific detail on a single claim.

Note that the JSON results are in a list, even if there is only one row. This is because some claims may have multiple parties, and thus will have multiple rows returned. See the bottom of this page for a full list of fields returned in the dictionary.
```
/claims/<claim_num>.json
```
You can get the same detail as the above for all claims you have access to, as well.
```
/claims/view_all_detail.json
```


### Fields
The following fields are returned for each row in the result set.
* accident_description
* accident_location
* adjuster
* catastrophe
* catastrophe_text
* claim_number
* claim_status
* company_name
* controlling_state
* in_hearing
* line_of_business
* lost_time
* low_company_name
* medical_manager
* nurse_case_manager
* other_claim_number
* party_name
* party_status
* payroll_state
* supervisor
* team_assistant
* utc_birth_date
* utc_closed_date
* utc_death_date
* utc_entered_date
* utc_hire_date
* utc_loss_date
* utc_lost_time_known
* utc_party_closed_date
* utc_party_opened_date
* utc_party_reopened_date
* utc_received_date
* utc_reopened_date
* utc_reported_date
