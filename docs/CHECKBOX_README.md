### Bindings

## pui-checkbox-group
Name      | Mandatory | Type        | Description
--------- | --------- | ----------- | -----------
[inline] | | boolean | true to indicate the checkboxes should be inline. Default to false.
[label] | | string | Label for the checkbox group.
[value] | | array &#124; string |
[name] | | string | Field name for the group of checkboxes. Auto-generated if not given.
[disabled] |  | boolean | Default to false.
(change) | | | Invoked when the group value is changed.<br/>Params: `PuiCheckboxChange` - `{source: PuiCheckBoxGroup, value: any}`

## pui-checkbox
Name      | Mandatory | Type        | Description
--------- | --------- | ----------- | -----------
[id] | | string | ID of the input, generated when not given.
[name] | | string | Field name. Ignored when used within a checkbox group.
[value] | | string | The value it'll be submitted as when checked.
[disabled] | | boolean | Display the input as disabled.
[label] |  | string | Label for the checkbox. Text content inside the tag will be used if not given.
[required] | | boolean | Indicates the checkbox must be included in submit, useful when e.g accepting terms before submit.
[checked] | | boolean | True to display the box as checked. Default to false.
(change) | | | Invoked when the checkbox is checked/unchecked.<br/>Params: `PuiCheckboxChange` - `{source: PuiCheckBox, value: any}`
