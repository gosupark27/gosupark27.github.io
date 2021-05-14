---
layout: post
title: Klojure Coans
---

## Opening Thoughts 

Wow, today has been an *intense* day of grinding out the koans. I am happy with my progress so far; however, I'm slowly but surely realizing how much depth there is to Clojure's deceptively simple nature. Of course, on the other hand, the *simple nature* can be viewed as an **elegant** approach to solving problems. Anyways, it's cool to see how Clojure is based on **lambda calculus**. Sounds daunting and complex but hopefully as I gain more experience working with Clojure I'll be able to see how *lambda calculus* has influenced the design of the language. 

As I have mentioned before in my previous post, the [Clojure docs](https://clojuredocs.org/core-library) are clutch and a valuable resource when it comes to solving the koans. 

*e.g. **syntax** for the **loop***  

`(loop [bindings*] exprs*)`

*e.g. **example** of how to use a **loop*** 
```
(loop [x 10]
  (when (> x 1)
    (println x)
    (recur (- x 2))))

;;=> 10 8 6 4 2
```

In other news, I am feeling a bit fatigued from today's session - mostly from not taking breaks in-between. My propensity, *whether for better or worse*, is that once I get invested in something that I enjoy, I go all out. So, unsurprisingly, it can be difficult for me to pump the brakes at times. With that being said, it is essential to take a pause and give myself time to recover. 

## Today's Tasks

1. Playing [poker!](https://poker.cleancoders.com/) - A user story estimate tool developed at Clean Coders.  
2. Met up with Gina - Dang, what can I say besides the fact that it was an awesome & enjoyable experience. Being able to talk to a fellow apprentice just has a different feel to it. Also, it is great that she is ahead of me, and has already been through a lot of the apprenticeship because if I ever feel frustrated or stuck I know that I have someone to talk to. During the video call we both talked about ourselves and got to know each other better. Ooh yeah also Gina graciously helped me with the functions koan that I was struggling with and saved me a lot of time & banging my head against the wall. _Thanks Gina!_
3. Work on Clojure Koans - Now, I have a deadline that is based on the computed *mean* from the poker app.

## Challenges
* Estimating how much time it was going to take me to go through all twenty-seven koans. To be honest, I may have estimated a bit too *optimistically...*
* Finding a *good time* to write my blog -- if I start too early I may miss some things that may happen later during the day. However, if I write too late then I will be heading off to bed at a later time. 
* Wrapping my head around **recursion** -- still working on that particular koan. 
* Wrapping my head around **HOFs (Higher Order Functions)** 
  * HOFs - A function that does at least one of the following: 
    * Takes one or more functions as an argument
    * Returns a function as a result/output

## TIL

### Business 
* How a **press release** can be utilized to give a more formal & well-polished feel to say a landing page that is being built for a client. 
* **Discovery Meeting:** *A form of investigative meeting used by consultants to learn more about a project's requirements.* 

### Poker
* Yes, Texas Hold'em is a great variant of poker, but I am referring to the poker app I used earlier today with Micah. 
  * For all user stories: Always provide **three estimates**. [*optimistic* | *realistic* | *pessimistic*] 
  * The reason for three estimates is because we want to have a holistic approach where we account for all possible risks and so the three *categories* are used to reflect that, i.e. **optimistic** when everything goes perfectly according to plan, **realisitic** a more balanced approach to the expected risks that will occur, **pessimistic** literally everything that can go wrong goes wrong, yikes. 
  * A user story is expected to be completed in a **single sprint** = one week iteration. 
  * A *single developer's* max capacity is **9 points** per week (*~36 hours*)
  * **1 point** is roughly worth a *half day's worth of work, e.g. **morning** or **afternoon*** --> **4 hours**
  * **PERT** 
  * >(Program Evaluation and Review Technique): A three point activity estimating technique that considers estimation uncertainity & risk by using three estimates to define an approximate probability for an activity's cost/duration. 
  * **PERT Formula:** ```PERT estimate = (Optimistic + (4 * Realistic) + Pessimistic)/6```

### Clojure
- **\\** (backwards slash) combined with a letter, e.g. `\C` represents the character literal *C*. 
- **Strings** in Closure are denoted by *double quotes*, whereas **Characters** are typically denoted by a *backwards slash*. 
- **/** (forward slash) can be used as a mathematical operator **OR** as a namespace separator, *e.g. `string/join`*
- Difference in *conjoining* a **vector** and a **list**. For a *vector* conjoining is at the end & for a *list* conjoining is at the beginning. 
- **List** can behave as a stack using `pop` and `peek`. 
- ***Equality** with collections* is done in terms of values, not reference
- The **Set** collection is behaves like a *set* in mathematical terms: *A set is a collection of well defined and **distinct** objects*. 
- A *map entry* is seen as a **key/value pair**
  - Furthermore, if a *hashmap* is treated as a sequence then the entries can be viewed as a sequence of `[k v]` pairs 
- `%` in an **anonymous function** is shorthand to reference the arguments passed into a function, *e.g. % or %1 refers to the **first** argument and then %2 is for second...%n for nth*
- 

## Reflections
Despite not knowing the fine details of what is being discussed during the standups, I am ejoying hearing everybody share about what they did yesterday, what their plans are for today, and, if there are any, obstacles & challenges they are facing. Also, I have fun listening to the business side of Clean Coders - there are useful insights to how a software consultancy company operates and deals with their clients. 

I realize that it will be difficult to fit *everything* I did on the post, so I have to choose the ones that have made the **biggest** impact on me. All said and done, writing these blog posts have been rewarding and a great way for me to reflect on my day.

In the end, I'm lucky to have Micah as my mentor and be a part of Clean Coders Studio. I will strive to push myself to become the best I can be whether that is becoming a better software craftsman, brother, or son. 
