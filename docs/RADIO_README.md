### Bindings

## pui-radio-group
Name      | Mandatory | Type        | Description
--------- | --------- | ----------- | -----------
[inline] | | boolean | True to indicate radio buttons should display inline. Default to false.
[model] | Y (if not using `[control]`) | any | Data model of the input binds to, `[name]` must be provided to indicate what portion of the data it binds to.
[name] | | string | Radio group field name.
[value] | | string | The value it'll be submitted as when checked.
[disabled] | | boolean | Display all fields as disabled.
[label] |  | string | Label for the radio group.

## pui-radio
Name      | Mandatory | Type        | Description
--------- | --------- | ----------- | -----------
[id] | | string | ID of the input, generated when not given.
[name] | Y (if using `[model]`) | string | Indicates what portion of the data it binds to.
[value] | | string | The value it'll be submitted as when checked.
[disabled] | | boolean | Display the input as disabled.
[label] |  | string | Label for the radio. Text content inside the tag will be used if not given.
