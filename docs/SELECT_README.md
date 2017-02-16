### Bindings
Name      | Mandatory | Type        | Description
--------- | --------- | ----------- | -----------
[id] | | string | ID of the input, generated when not given.
[name] | Y (if using `[model]`) | string | Indicates what portion of the data it binds to.
[value] | | string | The value it'll be submitted as when checked.
[disabled] | | boolean | Display the input as disabled.
[label] |  | string | Label for the input
[placeholder] |  | string | Placeholder text when empty.
[delimiter] | | string | The string to separate items by. When typing an item in a multi-selection control allowing creation, then the delimiter, the item is added. If you paste delimiter-separated items in such control, the items are added at once. The delimiter is also used in the getValue API call on a text `<input>` tag to separate the multiple values. Default to ','.
[textField] | | string | Field for text display
[valueField] | | string | Field for value storage
[searchField] | | string &#124; string[] | Field(s) for searching, default to textField
[allowCustomText] | | boolean | Allows the user to create new items that aren't in the initial list of options
[maxItems] | | number | The max number of items the user can select. 1 makes the control mono-selection, null allows an unlimited number of items. Default to 1.
[items] | | array | An array of the initial selected values, in the format of the object model. If not specified, it'll try to initialize from the `[control]` if provided.
[renderer] | | `SelectRenderer` | When customized text is required that `[textField]` is not sufficient. See below for the signature of `SelectRenderer`.
[customTextParser] | | function | In: `string`, Out: `any`<br/>When custom text is allowed, it's to parse the text into the object understood by the component.
[options] | | array | An array of the initial options available to select; array of objects.
[minChars] | | number | Minimum number of characters typed triggering the `(search)`. Default to 3.
(change) | | | Invoked when the value of the control changes.<br/>Params: `PuiSelectChange` - `{source: PuiSelect, value: any}`
(type) | | | Invoked when the user types while filtering options. Params: `string`
(search) | | | Invoked when new options have been loaded and added to the control. Params: `{query: string, callback: function}`

### SelectRenderer
Name      | Mandatory | Type        | Description
--------- | --------- | ----------- | -----------
[item] | Y | SelectItemRenderer | Custom renderer for the item dispaly in the field. See below for the signature of `SelectItemRenderer`.
[option] | | SelectItemRenderer | Custom renderer for the option to pick from.<br/>Default to `[item]` if not provided.

### SelectItemRenderer
Name      | Mandatory | Type        | Description
--------- | --------- | ----------- | -----------
[render] | Y | function | In: `(any, escape: (string) => string)`, Out: `string`<br/>`escape` argument is a function that takes a string and escapes all special HTML characters. This is very important to use to prevent XSS vulnerabilities.

### TODO
- Allow asynchronous [customTextParser]
