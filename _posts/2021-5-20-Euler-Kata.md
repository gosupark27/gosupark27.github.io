---
layout: post
title: Euler & Kata
---

## (is) The Way of Life

To my pleasant surprise, I have immensly enjoyed doing the bowling game kata. For me, it was the challenge of figuring out how I was going to "choreograph" my movements for my live performance on Monday. I had to think deeply and carefully about every keystroke I was making. My objective was to be efficient & quick with the code I was writing & my movement around the IDE. Perhaps this is a slight overkill but I am planning to memorize the `line:column` for certain parts of the program, so I can get there quickly in order to refactor the code or duplicate the lines. 

Anyways, it is a bit crazy to think that Euler #5 is rated at a **_5% difficulty_** when it seems to be pretty dang hard for me. Maybe I need to take my time with the problem and work out an angle where I can better understand the mathematical concept(s) behind the problem. It seems like for all these euler problems so far, there is always some kind of clever pattern or trick you can figure out and utilize to effectively solve the problem. Trying to figure that out has been a challenge and has given me the biggest frustration, if I am being honest. However, like all things with practice and time it will get better. 

## Today's Tasks
1. Euler #5
2. Bowling Game Kata 

## Challenges

### Euler 
- My initial solution worked up to the range `1 - 18` in terms of finding the minimum multiple; however, when I would go any higher, e.g. 19, 20 the program would stall out. 
- Regarding the pattern with the multiples figuring out how to get use `range` to get the multiples of a particular number. 

### Kata 

- Finding the right screen recording software. 
  - Making sure the quality is good. 
  - Also, making sure the font size is big enough since my desktop monitor screen is large. 
- Minimize the number of typos and pauses - I should be able to recall what to type without any issues 

## TIL

While solving euler problem #5 I came across a blog post that talked about a pattern that emerges when observing the smallest multiples divisible by a range. 
```
1 - 1
1 2 - 2
1 2 3 - 6
1 2 3 4 - 12
1 2 3 4 5 - 60
1 2 3 4 5 6 - 60
1 2 3 4 5 6 7 - 420
```
When looking at the **_next minimum number_** that is _evenly divisible_ by **all** the numbers within that range that number happens to be a **multiple** of the previous minimum number.

E.g. When finding the minimum number that is **evenly divisible** by `1 - 7` the number `420` is a multiple of `60` ( _the previous **minimum number**_). 

Also, the _subtle_ (at least for me at that time) difference between `(drop 1 (range 0 10 2))` vs. `(range 1 10 2)`. When I viewed both lines of code it seems like `drop 1` and starting the range at **1** were both accomplishing the same thing - **to drop the zero** from the range. However, since we are applying a `step` to the range it literally makes _all the difference_. 

```
user => (drop 1 (range 0 10 2))
;; 2 4 6 8 
user => (range 1 10 2)
;; 1 3 5 7 9
```



## Reflections

It's funny how the solutions to some of the Euler problems are seemingly so obvious and simple but when it is a novel problem it can take a while before you can successfully derive a solution to the problem. Often times this challenge of trying to grasp the underlying concepts can be a struggle and frustrating but it is the best path to growing and learning, in my opinion. It is by overcoming these obstacles do you achieve a deeper understanding of the problem because had you taken the easy way out and went straight to the solution you would inevitably gloss over some subtle detail that is critical to the understanding of the solution.
