angular-multiselect-searchtree
=============================

A native Angular multi select tree. No JQuery.
Original: https://github.com/kjvelarde/angular-multiselectsearchtree

#### Demo Page:
http://htmlpreview.github.io/?https://github.com/mtrawin/angular-multiselect-searchtree/blob/master/demo/index.html

#### Features:
Very Easy to Use:
- Plug and Play component
- Tree List
- Databind
- Filter/NoFilter by search textbox
- Checkbox
- Select one only or Multiselect
- NO JQuery

#### Design details:
Custom element using Angular Directive and Templating

#### Callbacks:
This is your onchange :)
e.g.

```html
data-callback="CustomCallback(item, selectedItems)"
```

##### Usage:
Bower installation:

```sh
bower install angular-multiselect-searchtree --save
```

Make sure to load the scripts in your html.

```html
<link rel="stylesheet" href="../dist/angular-multiselect-searchtree.min.css">
<script type="text/javascript" src="../dist/angular-multiselect-searchtree.min.js"></script>
<script type="text/javascript" src="../dist/angular-multiselect-searchtree.tpl.js"></script>

```

And Inject the module as a dependency in your angular app.

```
angular.module('[YOURAPPNAMEHERE!]', ['multiselect-searchtree', '....']);
```

###### Html Structure:

```html
<multiselect-searchtree
    multi-select="true"
    data-input-model="inputData"
    data-output-model="outputData"
    data-callback="CustomCallback(item, selectedItems)"
    data-select-only-leafs="true">
</multiselect-searchtree>
```

###### More options:

Show Select All / Clear All buttons:
```html
extra-buttons="true"
```

Hide the search box:
```html
filter-type="hidden"
```

Disable the search box:
```html
filter-type="disable"
```

Change search behaviour to also hide children that do not match your search:
```html
direct-search="true"
```

##### License

MIT, see [LICENSE.md](./LICENSE.md).

