angular-mention
======

[![Build Status](https://travis-ci.org/jeff-collins/ment.io.svg?branch=master)](https://travis-ci.org/jeff-collins/ment.io)
[![Coverage Status](https://img.shields.io/coveralls/jeff-collins/ment.io.svg)](https://coveralls.io/r/jeff-collins/ment.io)

@mentions and macros widget based on AngularJS.

To get started, add the following to your Controller to set up a scope variable called `people`:

```js
$scope.people = [
    {label: 'Joe'},
    {label: 'Mike'},
    {label: 'Diane'}
];
```

Then add this to your html:

```html
<input
    type="text"
    data-mentio
    data-mentio-typed-text="typedTerm"
    data-mentio-items="people | filter:label:typedTerm"
    data-ng-model="myval"
/>
```

Now you can type @ into your text field, and see a menu of choices.

There are many other options, including the ability to have multiple trigger characters, templates, binding your menu to an API, converting the selected item to markup, and more.
