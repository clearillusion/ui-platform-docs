### Bindings
Name      | Mandatory | Type        | Description
--------- | --------- | ----------- | -----------
[id] | | string | ID of the input, generated when not given.
[name] | | string | Name of the field.
[label] |  | string | Label for the input
[url] | Y | string | URL of the upload
[multiple] |  | boolean | True to indicate multiple files upload. Default to false.
[showQueue] |  | boolean | True to display the queue for files to upload. Automatically set to true when `[multiple]` is true. Default to false.
[showProgress] |  | boolean | True to display the file upload progress. Automatically set to true when `[multiple]` is true. Default to false.
[showDropZone] |  | boolean | True to display an upload zone to drop files to upload. Automatically set to true when `[hideFileInput]` is true. Default to false.
[hideFileInput] |  | boolean | True to hide the file input field. Default to false.
