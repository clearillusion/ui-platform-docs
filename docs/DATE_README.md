### Bindings
Name      | Mandatory | Type        | Description
--------- | --------- | ----------- | -----------
[id] | | string | ID of the input, generated when not given.
[disabled] | | boolean | Display the input as disabled.
[label] |  | string | Label for the input
[placeholder] |  | string | Placeholder text when empty.
[format] |  | string | Date format, e.g 'MM/DD/YYYY h:mm A'. Default to 'YYYY/MM/DD'.
[enableTimePicker] | N | boolean | Enables the time picker
[timePickerIncrement] | N | number | Time increment when time picker is available. Default to 30 minutes.
[minDate] |  | Date | The earliest day can be picked.
[maxDate] |  | Date | The latest day can be picked.
(change) | | | Invoked when date is picked or entered.<br/>Params: `PuiDateChange` - `{source: PuiDate, value: Date}`

### TODO
- Icon trigger the dropdown
