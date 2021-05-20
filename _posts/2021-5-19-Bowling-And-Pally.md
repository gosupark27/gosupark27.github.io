---
layout: post
title: Yo, banana boy!
---

## Title is a palindrome

Wow, out of all the euler problems I have solved so far, #4 has been the most rewarding because I was able to approach the problem from a high-level view on what functions I would need and what kind of data structure would be utilized in solving the palindrome problem. Of course, I had some help on what cool built-in library functions I could use to make my life easier, **_e.g. reverse, for, last, etc._**. 
Since I'm so excited about getting this solved, I might as well briefly elaborate on what I did to find the largest six-digit palindrome that is a _product of two **three digit numbers**_. That's a mouthful.

---

First, I created a test case to check `is-palindrome?` returns `true` if a number is a palindrome. 
```
(it "returns true if number is a palindrome"
    (should= true (is-palindrome? 5005)))
```
Here's the `is-palindrome` func:
```
(defn is-palindrome? [num]
  (let [num (vec (str num))
        rev-num (vec (reverse num))]
    (if (= 0 (compare num rev-num))
      true
      false)
    )
  )
```
Thanks to `reverse` I was able to easily reverse the number and then using `compare` check to see that both the original and reverse were matching. I must say I am slowly starting to add useful functions to my clojure repertoire, and I'm pleasantly surprised at my progress in Clojure despite feeling like I have not been putting in as much time into Clojure as I would have liked. 

Next, I created a `prod` definition: 
```
(def prod (for [num-1 (vec (range 1 1000))
                num-2 (vec (range 1 1000))]
            [num-1 num-2]))
```
`prod` represents the factors of all six digit products _of two **three digit numbers**_. I created two vectors and then took the **cartesian product** of the two vectors. 

Now, it was time to get the actual six digit products: 
```
(def six-digit-products
  (sort(set (map #(reduce * %) prod)))
  )
```
Since there were going to be repeats, I decided to use a set to get rid of any duplicates and I also sorted the set which I will explain why later on. 

At this point, I created the test case that was going to solve the problem and return _hopefully_ the correct answer to the problem. 
```
(it "Solves #4"
    (should= -1 (euler-4 -1)))
```
(Of course, the answer is not -1 but when I run the test and it fails -- the _actual_ correct answer will be shown)

Finally, in order to solve the euler problem this is what I did: 
```
(defn euler-4 [n]
  (last (filter is-palindrome? six-digit-products))
  )
```
Since the set has already been sorted when `six-digit-products` was defined I can simply use `last` to get the largest item in the set. 

In the end, I have learned a decent amount just from solving this one problem, and I hope that I can continue the good momentum I have built up and keep on learning!

## Today's Tasks
1. Bowling Game Kata 
2. Euler #4

## Challenges
* Definitely figuring out all the hotkeys that I can use in IntelliJ for the live kata performance
* Figuring out what kind of data structure to use for euler #4 -- holding all the products 
* Converting the **digit** `-->` **string** `-->` **vector** -- essentially, figuring this part out was new to me and an interesting way of approaching the problem. 

## TIL

### IntelliJ Shortcuts

| Shortcut  | Action |
| ------------- | ------------- |
| **`ctrl + tab`**  | Switch between tabs  |
| **`alt + enter`**  | Show Context Actions  |
| **`ctrl + alt + l`**  | Reformat Code  |
| **`ctrl+/`**  | Add/Remove Comment  |
| **`ctrl+g`**  | Go To Line:Column  |
| **`ctrl+shift+d`**  | Duplicate Entire Lines _(custom)_  |
| **`ctrl+d`**  | Duplicate Line/Selection  |
| **`ctrl+shift+right`**  | Split Vertically _(custom)_  |

## Euler

[I spoke about it at the beginning of the blog](#title-is-a-palindrome)

## Weekend on the Horizon 

I am looking forward to the Chicago trip ( _Saturday 05/22 to Wednesday 05/26_ ) that's coming up pretty soon! It'll be my first time visiting the **MidWestern** region of the USA. I'll be going there to visit my cousin who is matriculating to the University of Illinois at Urbana-Champaign this upcoming fall semester. He will be getting his masters in Instrumental Performance ( _I think...All I know is that he is joining their string quartert program_ ). Anyways, there's a decent list of things to do once we arrive to Chicago. 

My biggest concern is finding a good balance between working hard while I'm staying in Chicago and spending good quality time with my cousin since this is his first time moving out of state away from family. I'm happy for him and wish him the best on his new journey in Urbana. 
