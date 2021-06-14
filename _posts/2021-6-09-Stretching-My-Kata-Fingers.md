---
layout: post
title: Stretching My Kata Fingers
---

# Should You Warm Up Before You Start Coding?

~~**Warming up** helps prepare your body for aerobic activity. A **warmup** gradually revs **up** your cardiovascular system by raising your body temperature and increasing blood flow to your muscles.~~ Oh, sorry I got carried away talking about the wrong type of warm up. Anyways, during our apprenticeship meeting Gina and I were talking about the importance of warming up before diving into your user stories for the day. For example, doing your kata or euler problem is an excellent way to warm up because these warm up exercises gets your brain fired up and, especially with the kata, you are typing away based off of the muscle memory you have built up.  All in all, I think it is an excellent idea and I will be incorporating these ***coding stretches** *into my daily routine because who wants to get injured from doing a heavy coding lift. *Sigh*, sorry that was a horrible joke.  But on a more serious note, just like how before I start my hike/run or before I decide to lift heavy, I always make sure to warm up to avoid any injury & to give my self enough time to prepare and be able to perform at my best. 

# Today's Tasks

- Brief meeting w/Micah (Regarding time management & scheduling)
- Apprenticeship meeting w/Gina & Tatiana (Need to make sure to ping everyone beforehand!!)
    - Had a good discussion about how I can manage my time better (trim off time on things that are not top priority), the importance of Kata/Euler problems (as warm ups before heading into the user story), etc.
- Working on TTT (*human vs. human*)

# Observations

- This is a good lesson on why you do not simply copy and paste code that you find online. More importantly, you need to understand what the code is doing because when you copy & paste you are simply taking someone else's thinking & implementation and blindly trying to apply it to your problem. The main reason why I am saying all of this is because today I was working on getting the user's input from the console and there were some resources that told me to use the `read-line` func. However, the code example they provided was: `(println (read-line))`. More or less, I blindly copied this code and I was confounded as to why the number I entered was being repeated a second time.
    - Then I realized that this was happening because of the `println` func that was wrapped around the `read-line`
    - This was just a long-winded way of saying that it pays to fully comprehend the code that you found online & esp. so if you are going to be using it in your prod code.
- The principle of **DRY** (Don't repeat yourself) - I noticed that I was using a while loop on two separate occasions in my `-main` func, so I could refactor it such that I end up calling the func twice instead
    - All in all, I'm glad to have noticed that and I want to ensure that I try my upmost to practice writing clean code
    - As an aside Gina demonstrated the importance of not having duplicate code, so thanks for showing me that Gina!!

# Challenges

- Create an error validation func for making sure when the user inputs a `square` it is an int and not any other data type
- Currently, the game unexpectedly ends at the end of turn 8 and I am not able to place the final marker on the last remaining square (which would result in a tied game...)
- Furthermore, the game does not end when a winning row is made nor a tie
- After my **initial refactoring** of the `win?` func I ran into a new problem...
    - I used `let` to create a `board` variable that used a filter to take out all of the `\space` characters; however, that had the side-effect of

# TIL

- Maybe I'm overthinking this but when I was refactoring the `win?` func I realized that I could refactor in such a way that `mark` is not required in checking the equality of all **three squares** (*in a row*)  are the same mark. So, originally I was using this type of predicate to compare all three squares:
    
    ```
    (and (= mark (get board 1)) (= mark (get board 2)) (= mark (get board 3)))
    ```
    
- However, using the **transitive property** we can simplify the code above into something like this:
    
    ```
    (and (= (get board 0) (get board 1)) (= (get board 1) (get board 2)))
    ```
    
- The transitive property states that for \*all real numbers x, y, and z if \*\*x=y \*\*and \*\*y=z **then **x=z***
    
    - Hence, since we are already evaluating `square_0 = square_1` and `square_1 = square_2` the implication of the **_transitive property_** states that as long as the two comparisons hold true we can assert that `square_0 = square_2` **is also true** \ 
      - *Granted, something like this is a trivial application of the transitive property but this is one of the reasons why I enjoyed learning proofs back in college.*

# User Stories Schedule 

Micah and I met after our morning standup to have a quick discussion about the way I was prioritizing my user stories and how I was scheduling my time. Micah recommended that when I construct my schedule for the week, I should first work **backwards** and focus on tackling the **highest-risk user stories** first because the *sooner* I can explore the associated risks & determine whether or not those particular risks can be mitigated. Consequently, this approach gives me the greatest degree of flexibility and ensures that I will be able to deliver all my user stories by our next **IPM**. Thank you Micah for taking the time to give me invaluable advice on how I can better manage my time and I will be continually striving to refine my process of scheduling my week with the user stories I have planned to get done. On another note, I am pleased with the progress I have been making and I hope I can continue to grow and learn.
