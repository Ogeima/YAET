# General principles of chaining

Now we are finally ready to talk about chaining!\
The whole point of the Eberban grammar is to combine a lot of predicates into one big predicate that has our expected meaning. One way of combining predicates is the process called chaining.

**Chaining occurs when two predicates are juxtaposed next to each other**, and it transforms those two predicates into one predicate **which has the same set of arguments as the original left predicate**.\
When more than two predicates are juxtaposed, chaining occurs from right to left as such : (X (Y Z))

The default chaining behavior of the left predicate is determined by its transitivity :
 - if the predicate ends with the letter “n”, “r” or “l”, **then it has an intransitive behavior and its e place will interact with the right predicate**.\
    → Examples include mian and meon and miun.
 - if the predicate ends with any other letter, **then it has a transitive behavior and its a place will interact with the right predicate**.\
    → The only example here is buri.

This trick with the ending letters to know if it is transitive or intransitive only works on root words (denoted by the tag @R in the dictionary). But don’t worry, every predicate we will encounter in this section will be a root word.

All the examples of predicates given above (mian, meon, buri, miun) have arguments which expect atoms. Atoms are a type of variable that represents something, an entity, object or concept. They are not predicates and don’t have a truth value.
However, there are also predicates which have arguments that are expected to be predicates themselves.\
For example :
gli(c, e, A) = [e] is happy about the [A] predicate being true\
 → the e argument of gli is an atom argument, whereas the A argument of gli is a predicate argument.

And depending on whether the argument which is supposed to interact during chaining (e when the left predicate is intransitive and a when the right predicate is transitive) is an atom or a predicate, chaining behaves differently.
