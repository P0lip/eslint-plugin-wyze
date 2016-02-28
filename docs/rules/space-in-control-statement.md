# Spacing inside control statements (space-in-control-statement)

Always put spacing in your control flow statements.

## Rule Details

This rule is more granular than [space-in-parens](http://eslint.org/docs/rules/space-in-parens). This rule is limited to control flow statements only. `If`, `For`, `While`, etc.

This rule will enforce spacing inside these statements.

The following patterns are not considered problems:

```js
/*eslint wyze/space-in-control-statement: 2*/
if ( true ) {
  // Do something...
}

for ( var i = 0; i < 10; i++ ) {
  // Do something...
}

while ( true ) {
  // Do something...
}

do {
  // Do something...
} while ( true )

switch ( true ) {
  // Do something...
}
```

The following patterns are considered problems:

```js
/*eslint wyze/space-in-control-statement: 2*/
if (true ) {
  // Do something...
}

for ( var i = 0; i < 10; i++) {
  // Do something...
}

while (true) {
  // Do something...
}

do {
  // Do something...
} while (true )

switch ( true) {
  // Do something...
}
```


## When Not To Use It

You can turn this rule off if you are not concerned with the consistency of spacing between parentheses.