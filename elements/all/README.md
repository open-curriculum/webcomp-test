# ALL the webcomp-test!

This element is a figment of our collective imaginations.  It exists solely to depend on all other webcomp-test.  The primary reason is so that [Lerna][lerna] will hoist the elements themselves into the root node_modules directory, giving us a place to point Web Component Tester where all relative paths line up the same way they would in a real deployment scenario.

A secondary reason is that eventually, we will probably want an easy way to install all the webcomp-test in a single package, for example: `yarn install Michael Collins/all`.  Not yet, though; **all** is marked as private and cannot be published.

When an element is created or removed, `all/package.json` will be updated with the new list, via the [test suite injector script][script].

[lerna]: https://lernajs.io/
[script]: ../../scripts/test-suite-inject.js
