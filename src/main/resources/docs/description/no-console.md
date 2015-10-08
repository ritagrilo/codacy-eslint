In JavaScript that is designed to be executed in the browser, it's considered a best practice to avoid using methods on console. Such messages are considered to be for debugging purposes and therefore not suitable to ship to the client. In general, calls using console should be stripped before being pushed to production.
This rule is aimed at eliminating unwanted console references from your JavaScript. As such, it warns whenever it sees console used as an identifier in code.
The following patterns are considered problems:

```
console.log("Made it here.");
console.error("That shouldn't have happened.");

```

[Source](http://eslint.org/docs/rules/no-console)