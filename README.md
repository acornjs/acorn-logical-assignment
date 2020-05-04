# Logical assignment support for Acorn

[![NPM version](https://img.shields.io/npm/v/acorn-logical-assignment.svg)](https://www.npmjs.org/package/acorn-logical-assignment)

This is a plugin for [Acorn](http://marijnhaverbeke.nl/acorn/) - a tiny, fast JavaScript parser, written completely in JavaScript.

It implements support for logical assignments as defined in the stage 3 proposal [Logical Assignments](https://github.com/tc39/proposal-logical-assignments). The AST follows [ESTree](https://github.com/estree/estree/blob/master/experimental/logical-assignment-operators.md).

## Usage

This module provides a plugin that can be used to extend the Acorn `Parser` class to parse logical assignments:

```javascript
var acorn = require('acorn');
var logicalAssignments = require('acorn-logical-assignments');
acorn.Parser.extend(logicalAssignments).parse('x ||= y');
```

## License

This plugin is released under an [MIT License](./LICENSE).
