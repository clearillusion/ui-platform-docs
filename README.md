## P2 UI Platform based on Angular

[![npm version](https://badge.fury.io/js/%40p2%2Fstartup.svg)](https://badge.fury.io/js/%40p2%2Fstartup)

<img alt="P2ES" src="http://info2.p2energysolutions.com/rs/p2energysolutions/images/logo.png" width="60">

P2 UI Platform is a reusable UI platform for P2ES to build web applications with common standards and toolings. It is based on Angular.

**Vision: To build an atomic, reusable component platform for P2 Energy Solutions to consume.**

## Setup

* Ensure you have Node 6.9.1 or up and NPM 3+ installed.
* Install Angular CLI `npm i -g @angular/cli@latest`
* Install Typescript `npm i -g typescript`
* Install Node packages `npm i`
* Build vendor scripts and stylesheets `gulp build`
* Run local build `ng serve`

## Table of Contents

* [Getting Started](docs/GETTING_STARTED.md)
* [Developer Guide](docs/DEVELOPER_GUIDE.md)
* [Running Unit Tests](#running-unit-tests)
* [Releasing](docs/RELEASE.md)
* [Changelog](docs/CHANGELOG.md)
* [Quickstart](https://github.com/p2es/platform-quickstart)

## Components included in P2 UI Platform

P2 UI Platform contains a variety of components that are a part of P2 Platform design language.

| Feature | Template | Status | Docs | Issue
|---|---|---|---|---|
| Button | `<pui-button>` | `beta` | [readme](docs/BUTTON_README.md) | - |
| Checkbox | `<pui-checkbox>` | `beta` | [readme](docs/CHECKBOX_README.md) | - |
| Date | `<pui-date>` | `beta` | [readme](docs/DATE_README.md) | - |
| Date Range | `<pui-daterange>` | `beta` | [readme](docs/DATERANGE_README.md) | - |
| File | `<pui-file>` | `beta` | [readme](docs/FILE_README.md) | - |
| Date Range | `<pui-form>` | `beta` | [readme](docs/FORM_README.md) | - |
| Grid | `<pui-grid>` | `beta` | [readme](docs/GRID_README.md) | - |
| Input | `<pui-input>` | `beta` | [readme](docs/INPUT_README.md) | - |
| Navigation | `<pui-nav>` `<pui-nav-item>` | `beta` | [readme](docs/NAVIGATION_README.md) | - |
| Portlet | `<pui-portlet>` `<pui-portlet-header>` `<pui-portlet-body>` | `available` | [readme](docs/PORTLET_README.md) | - |
| Radio | `<pui-radio>` | `beta` | [readme](docs/RADIO_README.md) | - |
| Select | `<pui-select>` | `beta` | [readme](docs/SELECT_README.md) | - |
| Tab | `<pui-tabs>` `<pui-tab>` | `available` | [readme](docs/TAB_README.md) | - |

## Running unit tests

```bash
ng test
```

## Browser Support
P2 UI Platform is built on a Bootstrap Grid System, so the current browsers are supported in order or recommendation:

#### Current version - 1 for the following:

|   | Chrome | Firefox | Safari | Edge* | Mobile Chrome* | Mobile Safari* | IE11
|---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| __Supported__ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |

*Indicates limited testing & lower priority
