Before explaining chaining, lets see how predicates are defined in the [Eberban dictionary](https://eberban.github.io/eberban/web/dictionary.html#).

Here are four examples :
 - mian(c, e)    = [e:tce* pan] is a cat / field / member of family Felidae
 - meon(c, e)    = [e:tce* pan] is an apple
 - buri(c, e, a) = [e:tce pan] eats [a:tce pan]
 - miun(c, e)    = [e:tce* pan] sleeps

The word before the parentheses is the Eberban word that represents the predicate. It is the vocabulary that will be used in sentences (mian, meon, buri, etc).

The different letters surrounded by parentheses are the arguments that the predicate expects. They can be separated into two categories :
- **the context argument c**, which is implicit and handled automatically by the grammar. It carries information about the context such as tense, location, etc. For now you don’t need to worry about it.
- **the explicit arguments** : those are the ones that interact with the grammar. They are always in this order :
	→ the first one is called e
	→ the second one is called a
	→ the third one is called o
	→ the fourth one is called u

Finally, after this equal sign follows the definition of the predicate in plain English, where arguments previously found between parentheses are now between brackets. For now, you don’t need to understand the types of the arguments (which are expressed after the colon, for example *:tce\* pan*)

So to recap, here what you should be understanding when looking at that strange definition for mian :\
mian(c, e) = [e] is a cat (in the context [c])

*Quick reminder* : mian is a predicate that expects one argument (if we discard the context argument c) : so **mian is a property**.
