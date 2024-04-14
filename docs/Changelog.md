Below will list releases and their changes.

Please note that non-major version releases will rollup into the current endpoint
(e.g. release v1.1.0 will roll into `v1/`).

* v0.0.0
  * Initial release.
* v1.0.0
  * Changes to financial calculations including new `reserves/` field of `incurred_loss`
  and full fees for `incurred_indemnity`, `ptd_expense`, `reserve_expense`, and `incurred_expense`.
* v1.0.1
  * Party name consistency changes; will now also yield `"Unknown"` instead of `NULL`.
