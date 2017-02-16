### Bindings
Name      | Mandatory | Type        | Description
--------- | --------- | ----------- | -----------
[id] | | string | ID of the input, generated when not given.
[value] | | string | The value it'll be submitted as when checked.
[disabled] | | boolean | Display the input as disabled.
[label] |  | string | Label for the input
[placeholder] |  | string | Placeholder text when empty.
[format] | N | string | Date format, e.g 'MM/DD/YYYY h:mm A'. Default to 'YYYY/MM/DD'.
[enableTimePicker] | N | boolean | Enables the time picker
[timePickerIncrement] | N | number | Time increment when time picker is available. Default to 30 minutes.
[startDate] | N | Date &#124; moment object &#124; string | The start of the initially selected date range
[endDate] | N | Date &#124; moment object &#124; string | The end of the initially selected date range
[ranges] | N | array | Set predefined date ranges the user can select from. Each key is the label for the range, and its value an array with two dates representing the bounds of the range
(apply) | | | Invoked when values are applied.<br/>Params: `{start: Date, end: Date}`

### TODO
- Icon trigger the dropdown
