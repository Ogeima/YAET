# Predicate chaining

### Theory

You learned that arguments can either be atom arguments or predicate arguments.
In the previous section, you discovered the basics on how to chain an atom argument, let’s now explore chaining with predicate arguments...

First things first, in the dictionary, predicate arguments are denoted between parentheses.\
For example :\
 - tcu(c, e, A) = [e:tcui p] is the (non-empty) set of all things that individually satisfy **A:(tca p)**

The number of arguments inside the parentheses indicates the expected number of arguments for a predicate that could be linked with that slot.
For example :
 - the A argument of tcu expects a 1-argument predicate (a property)
 - cekme(c, e, A) = [e:tce p] differs in what they individually satisfy relation A:(tca a, b)
    → the A argument of cekme expects a 2-argument predicate (a relation)

You will also encounter 0-arguments predicate, such as in :\
gli(c, e, A) = [e:tce* pan] is happy about A:() being true

You might me thinking :
“But wait, isn’t a predicate without arguments simply a proposition ?”, and you would be right.
However, don’t forget the existence of the context argument. So technically speaking, a 0-argument predicate is a predicate of the context argument.

Now that we know how predicate arguments are defined, let’s talk about the chaining process for them :

1) Depending on the left predicate’s transitivity, we know which of its slots interacts with the right predicate (e for intransitive predicates and a for transitive predicates).
2) The AMR reduces the right predicate to make it match the expected number of arguments required by the predicate argument of the left predicate.
3) Finally the predicate resulting of the chaining is the same predicate as the left one, expect its e or a slot is said to be equivalent to the right reduced predicate.\
The left predicate's argument linked to the right predicate does not disappear : **re that the resulting predicate of any chaining process has always the same arguments as the left predicate**.

Let’s take an example and try to decipher the sentence : “mi gli mo kini e ber ban.” *(e ber ban is a compound to mean “the erbanic language”, just imagine it as being a property with an intransitive behavior)*

Here is the vocabulary you don’t know yet :
 - mi(c, e) = [e:tce* man] is I / me / the speaker(s)/narrators(s)\
	 → mi is not a predicate but a particle of the MI family, however, for now imagine it as an intransitive predicate. (you will learn later that **the transitivity of particles must be learned by heart**)
 - mo(c, e) = [e:tce* man] is you / a listener\
	 → same thing as “mi”
 - kini(c, e, a, o) = [e:tce* pan] (student) learns / studies [a:tce* man] from [o:tce* pan] (teacher)

Now let’s do it.
1) You must be comfortable chaining [ mo kini e ber ban ] by yourself as it is all atom chaining.\
	→ you should get the predicate : “e is you AND e learns Eberban from someone”
2) Now let’s chain (gli (mo kini e ber ban))
	1) gli is transitive as it ends with the vowel i. Thus its A argument will interact with the predicate (mo kini e ber ban).
	2) The A argument of gli expects a 0-argument predicate. However the right predicate has 1 argument : “e is you AND e learns Eberban from someone”.\
    So the AMR reduces it by filling its e argument by an existential variable. The right predicate thus becomes : “there is something which is you and which studies Eberban from someone (in the context c)”.
	3) Now we can chain the two predicates by establishing that the A argument of gli is equivalent to the right predicate.\
        → The resulting predicate is : “e is happy about A being true AND A is the predicate : there is someone who is you and who studies Eberban from someone”. Remember that this resulting predicate has still 2 arguments : e and A.
4) Now we simply need to chain (mi (gli mo kini e ber ban)) using the e atom argument of mi (intransitive).\
It should be pretty simple, just remember that the right predicate in atom chaining always must be reduced to 1 argument. So (gli mo kini e ber ban) become “There exists something named A AND e is happy about A AND A is the predicate : there is someone who is you and who studies Eberban from someone” before the chaining with “mi”.
5) The resulting big predicate is : “There exists something named A AND e is me AND e is happy about A AND A is the predicate : there is someone who is you and who studies Eberban from someone”.\
And that big predicate only has e as its argument. After the AMR has converted this predicate into a proposition we get our final result :
*“There exists an A and there exists something which is me and which is happy about A being true and A is the fact that in context c there is someone who is you and who learns eberban from someone”*.

Which in more standard English means : “I am happy that you are learning Eberban.”

There you go, it is as easy as that ! You can now start to formulate pretty complex sentences !
In the next section we will learn some more advanced chaining techniques.
For example, you may be wondering  how to chain the o place of kini…

### Practice

You can try to decipher those sentences !

1) mi dona tcu mian.
2) zmer tcu mian.
4) mi katmu mi buri meon.
3) me jene fniu tcuin.
