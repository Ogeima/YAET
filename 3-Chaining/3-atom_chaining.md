# Atom chaining

### Theory

If the argument selected for chaining (remember e or a depending on the transitivity of the left predicate) expects an atom, then the right predicate will first be changed so that it has exactly one argument : e (this change is done through AMR by filling the other arguments by existential variables), and then the result of the chaining will be a predicate made from a combination of the left and the right predicate where the selected argument of the left predicate is shared with the e argument of the right one.\
Lets take a few example to make this more clear :

Lets examine the chaining process in the sentence “mian miun”.
1) Take a look at the left predicate : is it transitive ? intransitive ?\
Because mian ends with the letter n, it has an intransitive behavior. Thus, the argument of mian that will interact with miun will be e.
2) So the e argument of mian and the e argument of miun will be shared.
3) Does the right predicate have exactly one argument (the e argument) ? Yes! So no need to use the AMR, great!
3) Now we can share the arguments and we end up with the predicate “e is a cat / field / member of family Felidae AND e sleeps”.
4) There is only one big predicate left, so the AMR fills every variable with an existential variable (“there exists something”).
5) We get our final proposition (which can be true or false, for example the speaker could be lying) which has the meaning : “there exists something which is a cat and which sleeps”. And this proposition has the same meaning as “a cat sleeps”.

There you go ! Your first Eberban sentence : “a cat sleeps” → “mian miun”.


Let’s take another slightly more difficult example to be sure everything is clear.\
Try to go through the same process as before to understand the meaning of “mian buri meon”.

Here is the solution :
1) Three predicates are strung one after the other, but chaining works on only two predicates at a time. So we start from left to right as such : (mian (buri meon)).
2) Lets apply chaining on “buri meon” :
	1) Look at the left predicate : is it transitive ? Intransitive ? Because it does not end with the letter “n”, “r” nor “l”, it has a transitive behavior. Thus its a argument will interact with meon.
	2) So the a argument of buri is shared with the e argument of meon.
	3) Does the right predicate (meon) have only one argument ? Yes, so no need to change anything with the AMR.
	4) We share the arguments and we get the new predicate, result of the chaining of buri and meon : “e eats a AND a is an apple”
3) We now need to chain mian with our new right predicate “e eats a AND a is an apple”
	1) Look at the left predicate : is it transitive ? Intransitive ? Because it ends with the letter n, it has an intransitive behavior. Thus its e argument will interact with “e eats a AND a is an apple”.
	2) So the e argument of mian will be shared with the e argument of “e eats a AND a is an apple”.
	3) Does the right predicate only have one argument ?\
	No ! So we need to transform this predicate so that it only keeps its e argument. AMR does the job by filling every other argument with an existential variable (here only the a argument).\
	Our new right predicate is now “e eats something that exists and that is an apple” which can be rephrased as “e eats an apple”.
	4) We can now share the mian’s e argument with the e argument of “e eats an apple”. We get the resulting predicate : “e is cat AND e eats an apple”

5) Now that our entire sentence has been reduced to only a single predicate, we can perform one last time the AMR on it, to get the proposition : “there exists something which is a cat and which eats an apple”. This proposition can be rephrased as “A cat eats an apple” (which is probably false).

There you go! If you understood correctly those two examples, then you will be able to reproduce the same logic on any sentences (with only atom chaining of course, we haven’t covered predicate chaining yet) ! You can now even start to create your own simple sentences.


### Practice

Here is some new vocabulary:

 - dona(c, e, a) = [e:tce* pan] likes [a:tce* man]
 - pra(c, e, a) = [e:tce* pan] loves [a:tce* man]
 - zun(c, e) = [e:tce* pan] is a boy / man / male (gender)
 - zin(c, e) = [e:tce* pan] is a girl / woman / female (gender)
 - zear(c, e) = [e:tce* pan] is a book
 - fleon(c, e) = [e:tce* pan] is music

Try to create the following sentences. (Do not hesitate to recreate the same process as shown above. Doing it by yourselves a few time will greatly improve your comprehension).

1) A boy likes books (Eberban predicates are not singular or plural by default)
2) A girl likes music.
2) A girl loves a boy.
