"use strict",
(Always at beginning)

## Use Strict!

`"use strict";`
The "use strict" directive switches the engine to the “modern” mode, changing the behavior of some built-in features. Strict mode is enabled by placing `"use strict"`at the top of a script or function. Several language features, like “classes” and “modules”, enable strict mode automatically.

## Where to put scripts

Only the simplest scripts are put into HTML. More complex ones reside in separate files.
The benefit of a separate file is that the browser will download it and store it in its cache.

# JS Rules

- Never declare multiple variables in one line. Although multiline stile is possible as stated below:

```
let user = 'John',
  age = 25,
  message = 'Hello';
```

## Variables

### `let`

-Case MATTERS//cAsE mATTeRs

- camelCase
- no hyphens
- can not start with a number
- only symbols allowed are `$`and `_`

- there are reserved names like `let`, `class`, `return`, `function`, or all of these https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Lexical_grammar#Keywords

#### `const`

- cant (of course) be changed
- same naming as `let` apply

`UPPERCASE` - is only used for hard-coded constants. The Value of the constant is known before code execution and can therefore be named uppercase.

## Data Types

### number

-both integer and floating point

- `infinity`represents mathematical infinity ∞
- `NaN` represents a computational error
- math in JS is always safe and the worst that could happen is a `NaN a.k.a. NUmber not available`

### string

- must be surrounded by quotes
- double or single quotes do not matter
- `backticks`can help with for example `the result is \${1+2}`a.k.a extended functionality.

### boolean

- true or false
- This type is commonly used to store yes/no values: `true` means “yes, correct”, and `false` means “no, incorrect”.

### null

- In JavaScript, `null` is not a “reference to a non-existing object” or a “null pointer” like in some other languages.

### undefined

- undefined

### Objects and Symbols

#### typeof Operator

-The call to typeof x returns a string with the type name

## Browser: Document, Events, Interfaces

### DOM (Document Object Model)

- represents all page content as objects that can be modified
  -the `document` object is the main "entry point" to the page. We can change or create anything on the page using it.
  i.e.

```
// change the background color to red//
document.body.style.background = "red";

// change it back after 1 second //

setTimeout(() => document.body.style.background = "", 1000);
```

#### Dom living standard

https://dom.spec.whatwg.org/

### How to walk the DOM

http://javascript.info/dom-navigation

![picture](/resources/walkthedom.png)

### BOM (Browser Object Model)

- represents additional objects provided by the browser (host environment) for working with everything except the document.

````
alert(location.href); // shows current URL
if (confirm("Go to Wikipedia?")) {
  location.href = "https://wikipedia.org"; // redirect the browser to another URL
}
```
````
