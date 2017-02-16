### Bindings
Name      | Mandatory | Type        | Description
--------- | --------- | ----------- | -----------
[id] | | string | ID of the input, generated when not given.
[formGroup] | Y | [FormGroup](https://angular.io/docs/ts/latest/api/forms/index/FormGroup-class.html) |
[hideReset] | | boolean | hide the reset button
(submit) | | | Invoked when the form is submitted.<br/>Params: `[formGroup].value`
(reset) | | | Invoked when the form is reset. Form will be set to pristine & untouched status.
