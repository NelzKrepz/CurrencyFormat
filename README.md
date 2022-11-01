# Currency Formatter
### This is a modified [currency module](https://github.com/ihsandulu/rupiahnumerik) by [ihsandulu](https://github.com/ihsandulu/)

<br>

# » Usage
## Import Module
```html
<script src="https://api.hasannelz.repl.co/cdn/Currency.js"></script>
```

## Constructor
```js
new CurrencyFormat(number, prefix);
```

<br>

## Properties
### 〉 .num
```
Return the inputted number.
```
### 〉 .prefix
```
Return the inputted prefix.
```
### 〉 .thousands_sep
```js
Thousands separate.

Example:
.thousands_sep = '.'
```
### 〉 .formatted
```
Return formatted currency string.
```

<br>

## Methods
### 〉 .toCurrency()
```
Return the formatted currency string.
```
### 〉 .assignElement(element)
```js
Params:
- element: DOM element as string. 

Assign formatter to the DOM `<input>` element
```

<br>

## String.prototype
### 〉 .currencyFormat(prefix)
```js
Params:
- prefix: (Optional) the currency prefix.

Example:
"9000".currencyFormat('Rp. '); // Rp. 9.000

Return formatted currency string.
```

<br>

# » Example
```js
// Using class constructor
var number = 2000,
    prefix = 'Rp. ';
var Currency = new CurrencyFormat(number, prefix);

console.log(Currency.toCurrency());

// Using String.prototype
var num = "10000",
    prefix = "Rp. ";
var format = num.currencyFormat(prefix);
```