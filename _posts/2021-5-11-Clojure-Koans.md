---
layout: post
title: Klojure Coans
---

## Opening Thoughts 

Wow, today has been an *intense* day of grinding out the koans. I am happy with my progress so far; however, I'm slowly but surely realizing how much depth there is to Clojure's deceptively simple nature as I work through the koans. Of course, on the other hand, the *simple nature* can also be described as to be **elegant**. Furthermore, I have enjoyed how Clojure has a mathematical aspect that is based on **lambda calculus**. Hopefully, as I continue to delve deeper into Clojure, I'll be able to make more connections and through the process gain a deeper appreciation for Clojure.  

As I have mentioned before in my previous post, the [Clojure docs](https://clojuredocs.org/core-library) are clutch and a valuable resource when it comes to solving the koans. The provided examples and *syntax(?)* are helpful in deciphering & understanding how to apply them correctly.

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

I am feeling a bit fatigued from today's session mostly from not taking breaks in-between. My propensity, *whether for better or worse*, is that once I get started on something I am invested in, I want to maintain that momentum at full steam. So, unsurprisingly, it can be difficult for me to pump the brakes at times. With that being said, it is essential to take a pause and give myself ample time to recover in order to be ready for the *next sprint*. Anyways, let's move on to the next sections. 

## Today's Tasks

1. Playing [poker!](https://poker.cleancoders.com/) - It was cool to use an internal tool developed at Clean Coders to make an estimate on how long it would take for me to complete a user story, which in this case was finishing all 27 koans. 
2. Met up with Gina. 
3. Work on Clojure Koans. 

## Challenges
* Estimating how much time it was going to take me to go through all twenty-seven koans. To be honest, I may have estimated a bit too *optimistically...*
* 

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

## Reflections
Despite not knowing exactly all the fine details when my team members are sharing during the standup, I have always enjoyed listening to what everyone has done the day before, what their plans are for today, and, if there are any, the obstacles & challenges that they hae been facing. Also, I personally like listening to the business side of Clean Coders as it provides me some insights on how a software consultancy company operates and deals with their clients. 

In the end, I am immensely grateful for this opportunity to be an apprentice under Micah and be working for Clean Coders. My biggest desire is to be able to take full advantage of the resources and opporunities that are in front of me, so that I can become the best version of myself. Whether that is in the form of becoming a craftsman, son, or older brother. 
