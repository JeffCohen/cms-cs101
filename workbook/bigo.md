# Algorithmic Complexity

There are an infinite number of ways to solved any given problem.  

Computer science asks, which is the best?

## What Do We Mean By "Best"?

Suppose I showed you three different ways to shuffle a computerized deck of cards.  They all work - they all end up with a seemingly randomized deck of cards.  Which one would you consider to be the "best"?  What criteria would you use to judge one from the other?

A couple of possible criteria come to mind:

* Which one shuffles the cards the fastest?
* Which one uses less memory?

These can be loaded questions, because there are special cases which might skew the answer.

* If the deck of cards as already randomized, "shuffling" might need require any work at all.
* If a "card" can be simply represented as a pairing of number and suit, then we could use a lot less memory than if a card was defined as its number, suit, color, graphical image for the front, and graphical image for the back.
* What does it mean to "shuffle" a deck?  If the deck starts out in  order, and we just move one card out of order, is that sufficiently "shuffled"?
* If our shuffling algorithm always produces the "same" random order for every deck we're given, would that be ok?

Comparing solutions is a lot harder than it might seem.

## A Standard Way To Compare

In most situations, we care about speed over anything else.  Once speed has been solved, reducing memory consumption (or in general, any resource - disk space, CPU locks, etc.) becomes the next performance target.  But speed is paramount.

So how do we compare based on speed?  Well, we could simply run all of our proposed solutions and measure their performance.  And this is in fact the best approach.

But the crazy thing is that the speed of any particular function might not be constant; in fact, it almost always varies with the size of the input it's given. Shuffling a deck of 5 cards is going to be faster than shuffling a deck of 52 cards.

So our question now becomes, which solution performs the best when faced with the *worst* case (which usually means, a very large input size)?

The answer is sometimes counter-intuitive, so computer science also gives us a standard way to describe the performance of any function or algorithm.  And it turns out that most algorithm will fall into one of small handful of categories.

## `O()` Notation

In which we decipher the confusing O(n), O(log n), O(n2) notation....

Also called computational complexity

Characterizes the worst-case performance of an algorithm with respect to input size

Math shapes: cubic, quadratic, logarthimic, linear, flat


O(n)

O(log n)

O(n log n)

O(n^2)


How can we determine complexity of an algorithm we write?

Watch out for nested loops
