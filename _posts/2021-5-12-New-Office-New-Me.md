---
layout: post
title: New Office New Me
---

Consider why you underestimated.  What was harder than you thought?  What slowed you down?

## Let's Talk Office

Yesterday, I moved my home computer, chair and a couple of other belongings into my new office. Of course, making this move is a **risk** because there is no guarantee that the apprenticeship is going to work out and that's a decent amount of money I could have saved if I worked at home instead. However, from my experience there are certain moments in your life where you have to be willing to accept that risk and go all-in because this can be an opportunity that comes only once in your life. There have been times in the past where I have let those chances slip past my fingers because I was fearful or I was unwilling to adapt to the changing circumstances. Even now learning Clojure, a new languge, has been both rewarding and challenging these past couple of days. It is an opportunity for me to grow as a developer and because Clojure has a different programming paradigm learning and becoming proficient in this language will improve the way I approach problems and consequently how I would solve those particular problems. Ultimately, the office represents a space where I can focus completely on the apprenticeship, and for that reason alone it was and is worth the investment. 

## Today's Tasks

1. Work on Clojure Koans 
2. Write this blog posts & more specifically discuss about why I underestimated the time I thought it would take for me to complete Clojure Koans
3. Watched a [talk by Rich Hickey](https://www.youtube.com/watch?v=2V1FtfBDsLU)

## Challenges 
* **Recursion**. Especially, with how in Clojure there are two different ways of creating a recursive function. 
* Getting accustomed to new office environment & making preparations ( meal prepping for breakfast & lunch, commute times, etc. ) 
* Learning how to learn - sometimes I feel like when I reference a youtube video or a blog article that sort of gives the solution to a clojure koan exercise I feel like I cannot use or even glance at that resource because it would mean that I am a dirty cheater. However, today I have come to realize that the way I was approaching these kinds of resources was with the incorrect mindset. Granted, these resources are **not the first** things to go to when I get stuck but rather if utilized with the right intention can be a helpful teaching tool. 
  * To elaborate, my idea was that when I find myself stuck on a particular koan exercise I would allot myself a certain amount of time to try to figure it out on my own (only relying on clojure docs *( still clutch and awesome by the way )*) and if I still couldn't make any progress I would reference those said resources and be focused on comparing how they approached it & what their thought process was in finding the solution. Then I would try to implement their solution on my own and not just lackadaisically `ctrl + c` and `ctrl + v`
  * Also, I have readjusted the way I have been doing my koans. Instead of trying to *speed run* through the koan exercises, I have decided that once I figure out what the topic of the koan is going to be I will first do my research and learn all that I can on that particular topic ( *say like for an hour or for some predetermined amount of time* ) and then head into the koan. Then I would feel more confident in solving the exercises and also the exercises are a way of reinforcing what I have just learned -- sorta like in math class when you do your math set it is a way of putting into practice what you have just learned in class. 

## TIL 
- Clojure does not have a **for loop** like in other programming languages. Instead you utilize recursion to iterate through data or some data structure. Definitely sets Clojure apart from other languages. Pretty cool. Kinda edgy. At least it forces me to get better & gain a deeper understanding of recursion. Win-win? 
- Also, anything, seriously like *anything*, in Clojure can be **treated as a data**. That's going to take a bit before it really sinks in. 
- Interestingly enough, there are only **two values** that are considered to be *logically false* in Clojure:
  1. `nil`
  2. `false`
      - Clojure's `false` is the java value of **`Boolean/FALSE`** (under the hood) 
- `defn <===> (def name (fn [params* ] exprs*))` 
- Two ways of doing recursion in Clojure (provided with examples): 
    1. The first way:  
  ```
  (defn pow [x n]
    (if (zero? n)
      1
      (* x (pow x (dec n)))) 
    ```
    2. The second way: 
   ```
   (defn pow [x n]
      (loop [k n p 1]
        (if (zero? k)
          p
          (recur (dec k) (* p x)))))
    ```

## Moving Forward...With Clojure Koans
- I need to improve my **time management skills**. A big reason as to why I slowed down in terms of progress ( *regarding the Clojure Koans*) was because a decent amount of time for the past few days were delegated to priorities that were related to getting myself acclimated/prepared for the apprenticeship, *e.g. finding/moving into a coworking space (I like to call it as my office haha), picking up a new pair of glasses, shopping for work clothes* **However,** on the bright side of things these were all one-offs, so moving forward I should have a better handle of my daily schedule. 
  - As a follow-up to what has been said...I have always been a night owl and preferred staying up late to get things done, but my mom has ( *rightfully* ) convinced me to switch things up and try waking up extra early and heading into the office to get some work done instead. 
  - In the past, I have done a **66 days challenge** where my mom, brother, and I would wake up around 4:00 AM make & drink some tea, change into our hiking attire, and head out to hike either Piestewa or Camelback - echo canyon trail ( which, by the way, is the *better & more challenging one. don't @ me* ). I surprised myself by successfully completing this challenge and realized that I can be a morning person if I put my mind to it. So...I really don't have a legitimate excuse as to why I couldn't adjust my daily routine. 
- Furthermore, I underestimated the time it would take to finish the twenty-seven koans because I based the difficulty of the koans on the first two koans I breezed through and as a result I was overlyconfident in how quickly I could get through all of it. Next time, I will do a thorough search through all the koans to get a better assessment on how many exercises there are per koan, what topics are being covered (easy/moderate/advanced), etc. 
- The koans starting from #19 to #27 had completely new topics that I was not familiar with and those topics required more time to learn and gain a decent understanding. Furthermore, there are always one or two exercises in any one of the koans which are particularly difficult and trying to solve one could sometimes take more time than solving the rest. Consequently, those two were the biggest factors in terms of obstacles that bogged down my progress thorough the Clojure koans. 
