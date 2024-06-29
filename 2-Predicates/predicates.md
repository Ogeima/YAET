The most important thing one must understand when starting to learn Eberban is that typical parts of speech that can be found in natural languages do not exist.
Indeed, **the only two parts of speech in Eberban are predicates and particles**. The latter will be covered latter, and we will focus on predicates for now.

Predicates are a concept directly taken from [Higher-Order Logic](https://en.wikipedia.org/wiki/Higher-order_logic), but before you run away, be aware that you don’t need any knowledge of mathematics nor mathematical logic to understand any of this document.

**A predicate is a logical relation between a given number of variables**.
For example, [x is a planet] is a predicate with one argument.
If you *apply* the variable “Earth” to its first argument, you get the proposition “Earth is a planet”, which is probably true.

When a predicate is linked to **only one variable**, it is said to be a **property**.
 → Examples include [x is a planet], [x is earth], [x is a cat], [x is asleep], [x is happy], …

When a predicate is linked to **two or more variables**, it is said to be a **relation**.
 → Examples include [x gives y to z], [x eats y], [x loves y], …
But remember “proposition” and “relation” are just more precise words than “predicate” : both [x is a planet] and [x gives y to z] are predicates.

Once every argument of a predicate has been full *applied*, the predicate evaluates to a **proposition**, which is another fancy word to mean : **a statement that can be either true or false (or unknown in the case of Eberban)**.
“Earth is a planet” is a proposition that - let’s be honest – is probably true.

**Predicates are the core building blocks of Eberban** : a combination of them can allow you to express anything you desire.

However, you must have noticed that it was previously mentioned that only predicates and particles are a part of speech in the language.
So what about variables ? To say “earth is a planet” in our previous example we used the variable (for example with the – arbitrary – name “e”) “e : Earth” and the predicate [x is a planet], and we somehow *applied* e to the predicate to get the expected proposition.
But how can this be done in Eberban without variables ?

Well let’s try to write “Earth is a planet” in **pseudo-Eberban** (no Eberban vocabulary is introduced yet in order to avoid confusing the beginner).
The trick is actually pretty simple : 

Let’s define two predicates :
 - [x is Earth]
 - [x is a planet]

We can now follow a simple process :
1) Apply an arbitrary variable e to [x is earth] → we get “e is the Earth”
2) Apply an arbitrary variable p to [x is a planet] → we get “p is a planet”
3) Then simply state that *e = p* → Thus, instead of [e is the earth AND p is a planet] we get [e is the earth AND e is planet]. (How is this “e = p” expressed in Eberban ? Well it is a part of the grammar that is done automatically by a process called **chaining** that we will explore later. For now just know we can achieve this by juxtaposing the two predicates like so : “earth planet”)
4) But we’re not done yet ! What we got is a predicate : [e is the earth AND e is a planet], but remember that we want to end up with a proposition (**every declarative sentence in Eberban ends up evaluating to a preposition**). And for that, a variable has to be applied to the e argument of this predicate. And that variable we need is precisely the idea of “something”. If we apply the variable “something” to the e argument of the predicate, we get the proposition : “something is the earth and this same something is a planet” which is basically a more convoluted version of the proposition : “Earth is a planet”.
And guess what, that “applying something” is done automatically in Eberban by a process called the **Arity Mismatch Resolution** (that we will also explore more in depth later) : **once the whole sentence has been combined into one only big predicate, an existential variable (“there exists something”) is applied to every argument of this predicate**.

To recap:
 - A sentence in Eberban is a combinations of multiple predicates
 - Those predicates interact together (for example by chaining) to form one big predicate
 - Any argument left in this big predicate is then replaced by an existential variable (by the AMR)
 - Because this big predicate has been fully applied, we get our final proposition - which can be true or false (for example “a cat is an apple” is probably false) – and which corresponds to the meaning of the sentence.

Because of this process, Eberban sentences have a slightly stranger phrasing compared to English sentences, but the **same meaning**, which is **always unambiguous due to the logic nature of Eberban and its deep connection with Higher-Order Logic**.
For example “mi buri” is interpreted as : “there exists something which is me and which eats (something else that exists)”, and has the same meaning as “I eat something”.
