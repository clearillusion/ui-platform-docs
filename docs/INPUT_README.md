### Bindings
Name      | Mandatory | Type        | Description
--------- | --------- | ----------- | -----------
[id] | | string | ID of the input, generated when not given.
[name] | | string | Indicates what portion of the data it binds to.
[value] | | string | The value it'll be submitted as when checked.
[disabled] | | boolean | Display the input as disabled.
[label] |  | string | Label for the input
[placeholder] |  | string | Placeholder text when empty.
[type] |  | string | 'text' &#124; 'hidden' &#124; 'password' &#124; 'number'
[icon] | | string | [Fontawesome icon string](http://fontawesome.io/cheatsheet/) without the 'fa-' prefix.

### Additional Bindings for Number Type
Name      | Mandatory | Type        | Description
--------- | --------- | ----------- | -----------
[step] | | number | Specifies the legal number intervals for an input field, for up & down arrows
