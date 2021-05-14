---
layout: post
title: Case Clojsed
---

## Ha Ha Ha

Okay, I admit that was a horrible attempt at a pun with Clojure but I couldn't help myself. My first step towards *Clojure enlightenment*.  Even though I struggled getting through some of the tougher koan exercises the pain was worth it in the end. But anyways, I am **happy** to be done with the koans and be able to successfully complete a task that was assigned to me.  As excited and motivated I am to give my best, I need to keep reminding myself that Rome was not built in one day, and likewise, this apprenticeship is all about taking consistent, small steps, even if at times it feels like I'm barely moving. This process reminds me a lot of what it is like going to the gym. When you are a noob and you have never worked out it is easy to make gains quickly but as your body gets accustomed to the hard work the linear growth you experience begins to dwindle and now you have to navigate through a new stage where progress is defined as an upward trend composed of dips and rises. 

## Today's Tasks

1. Finishing up on Clojure Koans 
2. Met up with Micah!
    1. Started **Euler**
    2. Bowling Game Kata

## Challenges 

* Need to go over what the deal with trandsucers are 
* For one of the Recursion koans I do not understand why we have to use the form `(rest (rest form))` instead of `(rest form)`   (*look at line 9*). Here's the code: 
```
1 (defmacro recursive-infix [form]
2  (cond (not (seq? form))
3        form ;;if the form is not a sequence it is just a raw number
4        (= 1 (count form))
5        `(recursive-infix ~(first form))
6        :else
7        (let [operator (second form)
8              first-arg (first form)
9              others (rest (rest form))]
10          `(~operator
11            (recursive-infix ~first-arg)
12            (recursive-infix ~others)))))
```
Okay, I literally just got it from looking at what I was typing. The reason why we call `rest` **twice** is because in our `let` we are assiging the first two elements of the form to `operator` and `first-arg`. Because of that `others` need to represent the `form` with `n-2` elements; hence, `rest` is called twice. As much as Clojure can be difficult to understand at first it is rewarding when you *finally* get it. 

## TIL 

- The difference between `vars` and `refs`. 
  - `vars` ensure safe use of mutable storage locations via *thread isolation*
  - `refs` ensure safe **shared** use of mutable storage locations via STM (software transactional memory)
    -  *This is where the concept of **transaction** comes into play*
    -  Also, Clojure transactions are like database transactions - they ensure that *all* actions on Refs are **atomic**, **consistent** & **isolated**. 
        - **<ins>Atomic:</ins>**  Every change to Refs made within a transaction occurs or none do.
        - **<ins>Consistent:</ins>**  Each new value can be checked with a validator function before allowing the transaction to commit.
        - **<ins>Isolated:</ins>**  No transaction sees the effects of any other transaction while it is running.
    -  Refs are bound to a single storage location for their lifetime
    -  Refs only allow mutation of that location to occur **within a transaction**
- ~~Speckle~~ **Speclj** Yeah...I don't know how to spell sometimes 😆 
- **TDD** (Test Driven Development) & **BDD** (Behavior Driven Development) 
  1. Create a test case 
  2. Run the test case & have it fail 
  3. Write the *bare minimum* to have the test pass 
  4. Write another test case `-->` back to **step 2** 
- TDD seems to be an iterative process and instead of coding first you write the tests first and based on the tests you produce the code. I am still getting a hang of this core concept, but I will definitely try my best to learn it and use it well. 

## Looking Ahead To TGIF 

I am slowly starting to piece together a solid schedule that fits my needs & also complements the needs of my mom & brother. Granted, I am fully dedicated to working full-time at Clean Coders but every now and then (*on Saturdays*) I have to go out to the business to help. With all of that said, I am planning to be in the office from 5 AM to 2 PM. I am not sure what time I am meeting with Micah on Fridays but depending on the time I'll accordingly make the appropriate adjustments. Anyways, with this change I want to maximize my productivity at the office and finish with enough time to go to the gym, take care of the house, etc. The future seems bright and exciting and I am grateful to be given this opportunity. 
