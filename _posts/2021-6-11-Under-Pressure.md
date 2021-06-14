---
layout: post
title: Under Pressure
---

# No Pressure, No Diamonds

I am starting to feel the heat in terms of being slightly behind my projected schedule because ideally I would have finished the **TTT human vs human** user story yesterday afternoon and for the evening I would have started some preliminary work on the **TTT AI user story**. Unfortunately, this is the reality I have to face and the most important thing to do in this situation is to ***adapt*** to the changing circumstances and be able to stay calm under pressure and focus on how to optimally spend my time. Going back to what Micah told me about *time management* the most **urgent**/**highest risk** user stories need to be done first and everything else can be done at a later time. Also, things like writing my blog can take a lower priority and I do not have to spend so much time in making sure it is well-written or the content amount is sufficiently large.

# Challenges

- Figuring out what base test case to write for the `minimax` func
    - Furthermore, what \*\*output \*\*should the `minimax` func return?
    - Initial thoughts: Have it return a `square` \- a number representing a board square
- Have to consider having a `depth` parameter to the `minimax` func
    - As the test cases get more specific/complex: Going from \*\*\*turn 9 \*\*\*to \*\*\*turn n \*\*\*where `0 <= n < 9`

# TIL

- **compare func** \- `(compare x y)`
    - `when x < y: -1`
    - `when x = y: 0`
    - `when x > y: 1`
    - similar to Java's `x.compareTo(y)`
    - However, it is \*\*different \*\*in the sense that it *writes for*: `nil` and compares numbers and collections in a \*\*type-independent manner \*\*

# Observations

- In TDD, having a solid test is \*\*pivotal \*\*& esp. having a good \*\*base case. \*\*This is because the base case will determine how the rest of the tests will be be derived.
- Sometimes after refactoring the production code, the output of a given function can change, which in effect raises a need to refactor the tests to match the new returned values.

# ToDos

- First test case: A game board that is on ***turn 9*** *\- e.g. only one empty square left to play*
- `GetEmptyBoardSquareIndices` func
    - Returns a vector of indices representing all the empty square boards for the `board` that is passed into the func

# When all the pieces finally come together

(Write about this when I finally have the minimax func up and running...hopefully TODAY)
