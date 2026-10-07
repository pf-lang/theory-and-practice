## The purpose and audience of this book

This is a book of short articles about Pipefish written at one time or another to explain aspects of it to people interested in programming language development, with the content originally delivered in tech talks, private emails, posts on social media, etc. The diversity of audience and occasion will I hope both explain and excuse any unevenness of tone, and the occasional repetition. These articles are compiled here for the same sort of audience: people who will appreciate the beauty and utility of Pipefish as a piece of language design.

It has very few pre-requisites, and those only in a few theoretical pages which are not dependencies of the more practical pages. The page [*Pipefish and the lambda calculus*](****) assumes that you know what the lambda calculus is; [*Latticial type systems*](****) assumes that you are familiar with algebraic type systems, and that you know what a lattice is; [*The next 698 programming languages*](****) supposes that you know what lazy evaluation is.

It does not contain implementation details, which can be found in the [`README.md` file](****) of the `source` directory of the main project repo, and in the `README.md` files of each subdirectory of `source`.

## Page contents

### 1. Pipefish in theory

This will explain some of the more abstract ideas behind Pipefish, and why its surface simplicity corresponds to some fairly simple math underneath too.

* [*Functional core, imperative shell*](****). Explains how we segregate state.
* [*Pipefish and the lambda calculus*](****). Sketches out how Pipefish is two short steps and a ton of sugar from being the lambda calculus. 
* [*Latticial type systems*](****). This describes the sort of type system that Julia and Pipefish have, a "naturally-occuring" system analogous to algebraic type systems, but simpler for the same reason that a lattice is simpler than a linear algebra. I explain the math. I also sketch out the practical benefit (in use-cases where it *is* a benefit) of such a system: i.e. that it allows you to use dynamism in powerful and principled and ergonomic ways when you want to, while allowing you to be uptight about types when you need to.
* [*The great panfunctor*](****). This takes a theoretical look at Pipefish's `for` loops, why they exist, and how they fit with the core semantics of the language. It contains a touch of PL history, and also some sarcastic mathematics, possibly the only example of the genre.
* [*The next 698 programming languages*](****). This contains a lot of PL history, and indeed mentions Fortran more often than Pipefish. It does in the process place Pipefish very precisely in the landscape of programming languages, and gives a very satisfying answer to the otherwise nagging question: "If this is such a good idea, why has no-one done it already?" This is also where we get a theoretical view of what role laziness plays in the language.

### 2. Pipefish in practice

* [*Why Pipefish needs to exist*](****). This explains why a whole new GPL is the best solution for some common real world problems that fundamentally can't be satisfied by existing languages, or by new or existing libraries or frameworks or DSLs. Obviously this is to some extent a tour of the more original-and-useful features.
* [*The world of Pipefish*](****). We talk about dependency injection and the One Untrue Api.
* [*The only good way to do SQL interop*](****). A short discussion of why most approaches to this are fundamentally flawed, with examples such as literally everything about the Java DOM.
* [*Roadmap*](****). This explains what needs doing to make Pipefish production-ready, and suggests how it should best be done.
* [*The last hero feature*](****). This shows how once the reference implementation of Pipefish and its standard libraries and other maintained features have been made production-ready, it will take very little money and/or effort to keep them that way in the face of technological change.

### 3. Appendices

* [*Bibliography*](****). Relevant links.
* [*The legend of the first compiler*](****). Fan fiction about John Backus, with wizards and elves.
