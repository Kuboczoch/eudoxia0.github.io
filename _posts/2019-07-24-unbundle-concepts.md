---
title: Unbundle Your Concepts
summary: Programming paradigms are bad.
tags: [plt]
---

>"Functional Programming" is great today precisely because it does not mean the
>same as it did in 1990 when it thoroughly sucked. Since then it adopted the one
>good thing about the "Object-Oriented Programming" hoax that really mattered:
>ad hoc polymorphism — through Type Classes. ([Tweet](https://twitter.com/Ngnghm/status/936677074517090304))
>
>OOP was a horrible package deal of good and bad concepts shoved together at
>random. Please "unlearn" by unbundling the concepts, not by throwing away the
>good ones with the bad ones. For instance, Haskell has great compile-time ad
>hoc polymorphism with Type Classes, thank you. ([Tweet](https://twitter.com/Ngnghm/status/932726785636257792))
>
>— François-René Rideau

Fare argues above that Haskell succeeded because it has type classes, which are
integral to the language, and underlie the machinery of monads and effectful
code in the language.

Whence type classes? From object-oriented languages. Wadler, in the 1988
[paper][wadler] that introduced the term:

>Type classes extend the Hindley/Milner polymorphic type system, and provide a
>new approach to issues that arise in object-oriented programming, [...]

Further down, the paper explains the motivation behind type classes in reference
to run-time polymorphism in Smalltalk.

Haskell is a jewel of orthogonal and principled language design, which most
would classify as sitting squarely in the domain of functional programming. And
yet this fundamental language feature comes from object-oriented languages.

Instead of thinking about OOP, we can think about:

- Behavioural subtyping
- Physical subtyping
- Contravariance and covariance
- [Concepts][cpp-concepts]
- [Method combinations][method-comb]
- Multiple dispatch

Instead of thinking about FP, we can think about:

- Pure functions
- Less strictly: preferring the creation of new objects rather than the mutation
  of existing ones, and preferring creating objects that represent actions
  rather than executing actions directly. (the [Command Pattern][command],
  nominally from OOP. Also [CQRS][cqrs]).

[wadler]: homepages.inf.ed.ac.uk/wadler/papers/class/class.ps
[cpp-concepts]: http://www.stroustrup.com/good_concepts.pdf
[method-comb]: https://www.cs.cmu.edu/Groups/AI/html/cltl/clm/node287.html
[command]: https://en.wikipedia.org/wiki/Command_pattern
[cqrs]: https://martinfowler.com/bliki/CQRS.html
