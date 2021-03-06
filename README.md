# angular-bootstrap-datepicker - [AngularJS](http://angularjs.org/) directives for the [bootstrap-datepicker](https://github.com/eternicode/bootstrap-datepicker)

At the moment, only the ["Component"](http://eternicode.github.io/bootstrap-datepicker/?markup=component) type is supported.

***

## Demo

Here's a working [jsfiddle](http://jsfiddle.net/cletourneau/kGGCZ/)
A more dynamic [demo](http://eternicode.github.io/bootstrap-datepicker/) of all the options is available for the original bootstrap-datepicker.


## Installation

Installation is easy, jQuery, AngularJS and Bootstrap's JS/CSS are required.
You can download angular-bootstrap-datepicker via bower:
`bower install https://github.com/rbatllet/angular-bootstrap-datepicker.git`

When you are done downloading all the dependencies and project files the only remaining part is to add dependencies as an AngularJS module:

```javascript
angular.module('myModule', ['ng-bootstrap-datepicker']);
```

You also need to include these files:
```html
<link rel="stylesheet" href="bower_components/bootstrap/dist/css/bootstrap.css" />
<link rel="stylesheet" href="bower_components/angular-bootstrap-datepicker/dist/angular-bootstrap-datepicker.css" />

<script src="bower_components/jquery/dist/jquery.min.js"></script>
<script src="bower_components/bootstrap/dist/js/bootstrap.min.js"></script>
<script src="bower_components/angular/angular.min.js"></script>
<script src="bower_components/angular-bootstrap-datepicker/dist/angular-bootstrap-datepicker.js" charset="utf-8"></script>
```

Make sure you use `charset="utf-8"` in your script tag if your browser (or those of your users) is displaying characters wrong when using another language.

## Settings

To use the directive, use the following code :

```html
<input type="text" data-ng-datepicker data-options="datepickerOptions" data-ng-model="date">
```

`ng-datepicker` : Indicates you want your input as a date picker.

`ng-options` : Object of the controller scope containing the [options](http://bootstrap-datepicker.readthedocs.org/en/latest/options.html) for your date picker.

`ng-model` : Variable of the controller scope to store the date. The date is currently store as a string, formatted according to the one set in ng-options.


For a working example, see https://github.com/cletourneau/angular-bootstrap-datepicker/blob/master/example/demo.html
