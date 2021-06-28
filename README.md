# ES2021Features
ES2021 Features 

#  Logical Assignment Operators

```JavaScript
// "Or Or Equals" (or, the Mallet operator :wink:)
a ||= b;
a || (a = b);

// "And And Equals"
a &&= b;
a && (a = b);

// "QQ Equals"
a ??= b;
a ?? (a = b);


#  Logical Assignment Operators

```JavaScript

const updateID = emp => {

  // We can do this
  if (!emp.id) emp.id = 1

  // Or this
  emp.id = emp.id || 1

  // Or use logical assignment operator.
  emp.id ||= 1
}

```JavaScript

function setOpts(opts) {
  opts.cat ??= 'meow'
  opts.dog ??= 'bow';
}

setOpts({ cat: 'meow' })


# Numeric Separators

```JavaScript

1_000_000_000           // Ah, so a billion
101_475_938.38          // And this is hundreds of millions

let fee = 123_00;       // $123 (12300 cents, apparently)
let fee = 12_300;       // $12,300 (woah, that fee!)
let amount = 12345_00;  // 12,345 (1234500 cents, apparently)
let amount = 123_4500;  // 123.45 (4-fixed financial)
let amount = 1_234_500; // 1,234,500
