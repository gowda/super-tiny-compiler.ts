[![tests](https://github.com/gowda/the-super-tiny-compiler/workflows/tests/badge.svg)](https://github.com/gowda/the-super-tiny-compiler/actions)

***Welcome to The Super Tiny Compiler!***

This is an ultra-simplified example of all the major pieces of a modern compiler
written in easy to read JavaScript.

Reading through [the architecture document](ARCHITECTURE.md) will help you learn about how *most* compilers
work from end to end.

### [Want to jump into the code? Click here](the-super-tiny-compiler.js)

---

### Why should I care?

That's fair, most people don't really have to think about compilers in their day
jobs. However, compilers are all around you, tons of the tools you use are based
on concepts borrowed from compilers.

### But compilers are scary!

Yes, they are. But that's our fault (the people who write compilers), we've
taken something that is reasonably straightforward and made it so scary that
most think of it as this totally unapproachable thing that only the nerdiest of
the nerds are able to understand.

### Okay so where do I begin?

Awesome! Head on over to [the architecture document](ARCHITECTURE.md).

### I'm back, that didn't make sense

Ouch, I'm really sorry. Let me know how it can be improved.

### Run
Setup CLI
```
$ npm link
```

Read input source from stdin:
```
$ echo '(add 2 (subtract 4 2))' | npx supertinyc
```

Read input source from file:
```
# contents of example.lisp
#
# (add 2 (subtract 4 2))
#

$ npx supertinyc example.lisp
```

Any number of files can be passed as arguments, each file will be compiled one after the other.

### Tests
```
$ npm test
```

---

[![cc-by-4.0](https://licensebuttons.net/l/by/4.0/80x15.png)](http://creativecommons.org/licenses/by/4.0/)
