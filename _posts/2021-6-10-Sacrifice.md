---
layout: post
title: Sacrifice
---

# Don't Want No Compromise

Recently, I have been listening to this song called *Sacrifice by Bebe Rexha* on repeat and even though the lyrics could be viewed as trite and insipid I interpreted the lyrics in a more abstract sense. For example, based on the lyrics, if there is something that you truly desire there is going to be some element of **sacrifice** involved and you have to be iron-willed; hence, there should be **no compromise**. Personally, this seemingly *random* thought is a relevant application to my situation where I have to be willing to sacrifice my time and other obligations in order to ensure that all of my user stories get delivered on time.   

# Challenges

- Debating between whether to use `(def combo)` or `(defn get-combo [board])`
    - When using `def` usually you are assuming that the value will more or less be \*\*\*static \*\*\*
    - On the other hand, `defn` seems to be more fitting if `get-combo` utilizes math/other functions to generate a vector of all the \*\*\*winning row combos \*\*\*

# TIL

- `some` func: returns the first logical true value of `(pred x)` for any x in `coll`
- `when - (when test & body)` evaluates the *test* and if ***true*** evaluates the *body* (in an implicit do)
- Obvious but it does not help to be reminded once again: `(not nil)` evaluates to `true`

# Observations

- When you properly decompose a problem into appropriate subproblems & write a good test suite to go along with the \*helper function \*that successfully solves that subproblem --> the end result is a concise, elegant line of code that solves that problem.
    - Slowly gaining a deeper appreciation of Clojure as it empowers you to write powerful code with few words.
- `some` func returns `nil` if there is \*\*no \*\*\*x \*in coll that returns \*\*\*true ***

# ToDos - What I Worked On

- Refactored `win?` func using the new helper functions: `get-combo` and `all-same-marker?`
- Create a map for end game message, e.g. `(def msg {:win "winner winner chicken dinner" :tie "cat's game!"})`
- (Not yet done) Refactor `get-nth-row` and get-board by using `partition` instead of `subvec`
    - This goes to show that there are different ways to get a problem done, but often times there is a more s*traightforward, simpler solution*

# Putting in the Work 

Overall, I'm glad how today went in terms of being able to stick to my schedule and focusing mainly on getting the **TicTacToe human vs human user story** completed. I believe I should be able to get it done by early Friday and the plan is to send my user story to Micah and Gina and wait for their thoughts/feedback. Obviously, there is a huge advantage to getting the user stories done **early **as it gives you enough cushion (*in terms of time*) to deal with any ***risks***.
