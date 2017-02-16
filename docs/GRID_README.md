### Bindings
Name      | Mandatory | Type        | Description
--------- | --------- | ----------- | -----------
[autoFit] |  | boolean | Gets columns to adjust in size to fit the grid horizontally. This will override all column width settings. Default to false.
[autoSize] |  | boolean | Auto-sizes **all** columns based on it's contents. Individual 'auto' size should be set per column.
[width] | | number &#124; string | Grid width in (number)px or string with '%'. Default to '100%'.
[height] | | number &#124; string | Grid height in (number)px or string with '%'. Default to 300.
[rowData] | | Array | Data to be displayed as rows in the table.
[gridOptions] | | `PuiGridOptions` | See available options below.
[selectionMode] | | string | `single` &#124; `multiple`
(select) | | string | Invoked when selection change happend. Params: array of the row data or empty if no row selected.
(rowDblClick) | | string | Invoked when a row is double clicked. Params: the selected row data.

### Grid Options
Name      | Mandatory | Type        | Description
--------- | --------- | ----------- | -----------
[enableColResize] |  | boolean | Column resizing. Default to false.
[enableSorting] |  | boolean |
[enableFilter] | | boolean |
[datasource] | | `GridDataSource` |

### Column
Name      | Mandatory | Type        | Description
--------- | --------- | ----------- | -----------
[header] |  | string | Column header
[field] |  | string | Data field for display
[sort] |  | string | Enable default sorting if specified. If the column is sortable but not by default, use `[sortable]` instead.. `asc` &#124; `desc`.
[width] | | number &#124; string | Column width in pixel or 'auto'. Default to 'auto'.
[headerRenderer] | | | Custom renderer for the header.<br/>Params: `PuiGridHeaderParams`: `{value:any, colDef:any}`
[renderer] | | | Custom renderer for the cell.<br/>Params: `PuiGridCellParams`: `{value:any, data:any, context:PuiGridOptions}`
[sortable] | | boolean | True to flag the column is sortable. `enableSorting` must be set to true in `gridOptions`. Default to false.
[comparator] | | | Custom comparator when sorting is enabled.

### TODO
- Grid grouping
- Grid filtering
- Grid inline edit
- Grid export to pdf/excel
