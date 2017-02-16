### Bindings
Name      | Mandatory | Type        | Description
--------- | --------- | ----------- | -----------
(select) |  |  | Invoked when a nav item is selected. Params: `PuiNavItem`(see below).

### Nav Item Bindings
Name      | Mandatory | Type        | Description
--------- | --------- | ----------- | -----------
[name] |  | string | Label for the item.<br/>If not specified, content inside the `<pui-nav-item>` will be used as label.
[routerLink] | Y | [RouterLink](https://angular.io/docs/ts/latest/api/router/index/RouterLink-directive.html) | String or array as long as supported by `RouterLink`.
[queryParams] | | {[k: string]: any} | Query parameters of the URL. Could be embedded in `[routerLink]`.
[fragment] | | string | Fragment of the URL. Could be embedded in `[routerLink]`.
