---
title: Unbundle Your Concepts
summary: Programming paradigms are bad.
tags: [plt]
---

Fare argues that Haskell became the most successful functional programming
language because it has type classes, which are integral to the language, and
underlie the machinery of monads and effectful code in the language.

Whence type classes? From object-oriented languages. Wadler, in the 1988
[paper][wadler] that introduced the term:

>Type classes extend the Hindley/Milner polymorphic type system, and provide a
>new approach to issues that arise in object-oriented programming, [...]

Further down, the paper explains the motivation behind type classes in reference
to run-time polymorphism in Smalltalk.

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
