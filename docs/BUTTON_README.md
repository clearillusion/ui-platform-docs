### Bindings
Name      | Mandatory | Type        | Description
--------- | --------- | ----------- | -----------
[type] | | string | 'default' &#124; 'submit' &#124; 'link'
[disabled] | | boolean | Displayed the button as disabled.
[icon] | | string | [Fontawesome icon string](http://fontawesome.io/cheatsheet/) without the 'fa-' prefix.
[buttons] | | array | Configuration for a button group, which each in the array same options as per button
[verticalGroup] | | boolean | Button group layout horizontally or vertically. Default to false, which is horizontally laid.
(groupButtonClick) | | | Invoked when a button within the button group is clicked. Params: button ID
