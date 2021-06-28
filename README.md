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
