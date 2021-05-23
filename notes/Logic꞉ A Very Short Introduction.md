---
title: 'Logic: A Very Short Introduction'
tags: [reading]
created: '2021-05-22T12:11:43.702Z'
modified: '2021-05-22T12:12:19.731Z'
---

# Logic: A Very Short Introduction

Graham Priest

<img src="https://images-na.ssl-images-amazon.com/images/I/71yl2An07pL.jpg" alt="img" style="width:400px;" />



# Table of Contents

[toc]

# Chapter Summary

## Validity: What follows from what?

> …the central aim of logic is to understand validity

Main ideas:

- A *valid inference* is when the conclusion follows from the premiss(es)
- A *deductively valid* inference is when there is no situation in which all premisses are true, but the conclusion is not
- An *inductively valid* inference is when the premisses offer reasonable grounds for the conclusion drawn, though not necessarily a conclusive one
- An *inference* is a piece of reasoning, where premisses are given as reasons for a conclusion

Might ability of reasoning & logic be understood similarly to Chomsky’s ideas of language?

How do we understand negation and truth?

How is it possible to evaluate a statement for all situations (similar to problem posed to the positivists)?

## Truth functions—or Not?

By writing sentences as single letters, it is possible to test the general form of the inference for validity in the abstract situation.



Main ideas:

- A *truth value* can be assigned to each sentence in a situation as T or F (true or false)
- A *truth table* can be constructed to assess inferences, define functions, etc. 
- The symbol for *negation* is “$\neg$” 
- The symbol for *disjuncton* (either…or…) is “$\lor$”
- The symbol for *conjuction* (both…and…) is “$\land$“ (can also be “&”)
- An inference is *vacuously valid* if the premises can never all be true together
  - There is still no situation where all the premises are true, and the conclusion is false (as the premisses are never all true)

### Writing arguments

Arguments can be written with the following formats:

- Premisses are written above a line, and the conclusion below it.

$$
\frac{Either\,the\,Queen\,is\,rich\, or \,pigs\,can\,fly \qquad The\,Queen\,isn't\,rich}{Pigs\,can\,fly}
$$

- As a series of (numbered) statements, where the last is the conclusion
  1. Either the Queen is rich or pigs can fly
  2. The Queen isn’t rich
  3. Pigs can fly

Problems with the logic in this example

1. It is *unsound* as not all the premisses are true (premiss 2 may be contested as false)
2. It is *invalid* even if 

This example is also *invalid*, as it is **not** the case that the Queen being not rich makes   

### Truth tables

1. The header row is what you are evaluating the truth value of in each column
2. Rows are treated as a unit, where the truth values of each row make up the truth values within the sentence
3. The final column is the conclusion, using the truth values from previous columns within the same row to evaluate it

Example:

A truth table for any sentence of the form “$\neg$a$\land$b” (this could be a sentence such as: the Queen isn’t rich, and pigs can fly)

| a    | b    | $\neg$a | $\neg$a$\land$b |
| :--- | :--- | :-----: | --------------: |
| T    | T    |    F    |               F |
| T    | F    |    F    |               F |
| F    | T    |    T    |               T |
| F    | F    |    T    |               F |

From this table, we can see that:

1. If “a” is true, then “$\neg$a$\land$b” is always false
2. If “b” is false, then “$\neg$a$\land$b” is always false
3. If the premisses (“$\neg$a” and “b”) are true, then the conclusion (“$\neg$a$\land$b”) is also true

Truth tables can be useful in this way.

For example, we can evaluate an argument such as $\frac{The\,Queen\,isn't\,rich \qquad Pigs\,can\,fly}{The\,Queen\,is\,rich\,and\,pigs\,can\,fly}\nonumber$ 



### $\neg$ negation truth table

| a    | $\neg$a |
| :--- | ------: |
| T    |   **F** |
| F    |   **T** |

### $\lor$ disjunction truth table

| a    |  b   | a$\lor$b |
| :--- | :--: | -------: |
| T    |  T   |    **T** |
| T    |  F   |    **T** |
| F    |  T   |    **T** |
| F    |  F   |    **F** |

### $\land$ conjunction truth table

| a    |  b   | a$\land$b |
| :--- | :--: | --------: |
| T    |  T   |     **T** |
| T    |  F   |     **F** |
| F    |  T   |     **F** |
| F    |  F   |     **F** |

### An example of vacuous validity

An example of a vacuously valid inference may be:
$$
\frac {q \quad \neg q}{p}
$$



| q    | p    |  q   | $\neg$q |     p |
| :--- | :--- | :--: | :-----: | ----: |
| T    | T    |  T   |    F    | **T** |
| T    | F    |  T   |    F    | **F** |
| F    | T    |  F   |    T    | **T** |
| F    | F    |  F   |    T    | **F** |

1. There is no situation where all the premisses are true
2. No situation where all premisses are true but the conclusion is false
3. $\therefore$ $\frac {q \quad \neg q}{p} \nonumber$ is a *vacuously valid inference*

However, see #

## Names and Quantifiers: Is Nothing Something?

Main ideas:

- A sentence *nP* is true in a situation if *n* has the property expressed by *P* in that situation

- $\exists$x(xP) is  true in a situation if there exists some object x, which is such that xP, in that situation
- $\forall$x(xP) is true in a situation if every object x, is such that xP, in that situation

Chapter 2[] looked at truth functions which add to or join whole sentences to make new ones. However, Many inferences work in a different way.
$$
\dfrac{Marcus\,gave\,me\,a\,book}{\,Someone\,gave\,me\,a\,book} \tag{1}
$$

Neither the premiss nor conclusion is made of parts consisting of a whole sentence. The logic behind the inference then is to do *within* the sentences, instead of *about* the sentences (predicate instead of sentence logic).



Sentences can be composed of a *subjet* and *predicate*. Consider the following sentences;

1. Marcus saw the elephant
2. Annika fell asleep
3. Someone hit me
4. Nobody came to my party

In these cases, the first word is the subject and the rest the predicate. In 3. and 4., the predicate is more ambiguous

- Who does “someone” refer to? It might not refer to the person who “hit me” if no one hit me, for example.
- What does “nobody” refer to?

An example of the type of results from ambiguous predicate logic is from *Alice Through the Looking Glass*

> “Just look along the road, and tell me if you can see … [the Messanger].”
>
> “I see nobody on the road,” said Alice.
>
> “I only wish I had such eyes,” the King remarked in a fretful tone. “To be able to see Nobody! And at that distance too! Why, it’s as much as *I* can do to see real people, by this light!”

When Alice says she can “see nobody” she does not refer to a person or anything, real or not. Words like “nobody”, “someone”, “evereyone” are called *quantifiers*. They are distinguished from nams like “Marcus”

In predicate logic, names are written as a lowercase latin leter, and predicates as an uppercase letter.

1. We can write *a* for Annika, and *F* for the predicate “fell asleep”
2. Convention places the predicate before the name, so we write the sentence “Annika fell asleep” as *Fa*

The sentence “Someone fell asleep” has a *quantifier* as the subject

1. The sentence is true if *some object*, x, fell asleep
2. We can write “Some object x is such that” as $\exists$x
3. We can write “some object x is such that x fell asleep” as $\exists$x  x*F* or $\exists$x(xF)

For the sentence “Everyone fell asleep”

1. We can write “Every object x is such that” as $\forall x$

2. We can write the sentence “Every object x is such that x fell asleep” as $\forall$x   x*F* or $\forall$x(xF)

“Nobody fell asleep” can be written “no object, x, is such that x fell asleep” as *$\neg\exists$x(xF)* 

- Nobody fell asleep means “it is not the case that somebody is happy”

We can reqrite (1) as:
$$
\dfrac{Gm}{\exists x (Gx)}
$$

- So it is clear that if *m* gave me a book, then some object in the relevant collection gave me a book

Similarly, we can rewrite the White King’s inference:
$$
\dfrac{\neg \exists x (xA)}{\exists x(xA)}
$$

### Application to a simple version of the Cosmological Agument

2. Everything has a cause
3. There must be a cause then, for everything 
4. This cause cannot be of the world, as it then would have a cause
5. The candidate for this First Cause is God

There is a logical fallacy

The sentence “Everything has a cause” is ambiguous:

- It can mean “everything which happens has some cause or another”, for every *x* there is a *y* such that *y* caused *x*
- It can mean “there is a (singular) cause for everything”, there is a *y* such that for every *x*, *x* is caused by *y*

1. $\forall$x $\exists$y (xCy)
2. $\exists$y $\forall$x (xCy)

These are not logically equivalent

- If we change C to be addition, and (x,y) the domain of real numbers, then
  1. is “for all real numbers x there exists a real number y such that x+y=10,” or “for every real number, there is another real number which can be added to it to make 10,” which is True
  2. is “there exists a real number y such that for all real numbers x,  x+y=10,” or “there is a singular real number which can be added to any other real number to make 10,” which is False

- The first claims that for every event *x* there exists a *y*, such that *x was caused by y*; the second claim states that there exists some *y*, such that every event *x* (everything), *x was caused by y*

