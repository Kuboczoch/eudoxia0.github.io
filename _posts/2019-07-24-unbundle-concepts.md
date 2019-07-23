---
title: Unbundle Your Concepts
summary: Programming paradigms are bad.
tags: [plt]
---

Fare argues that Haskell became the most successful functional programming
language because it has type classes, which are integral to the language, and
underlie the machinery of monads and effectful code in the language.

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

[cpp-concepts]: http://www.stroustrup.com/good_concepts.pdf
[method-comb]: https://www.cs.cmu.edu/Groups/AI/html/cltl/clm/node287.html
[command]: https://en.wikipedia.org/wiki/Command_pattern
[cqrs]: https://martinfowler.com/bliki/CQRS.html
