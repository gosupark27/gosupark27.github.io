---
layout: post
title: First Blog Post
---

## Setting expectations

Hello World! This is my first blog post and I am excited to utilize blogging as a way to document my apprenticeship at Clean Coders. Mr. Tom Preston-Werner succinctly summarizes the joy and benefits of writing *or blogging*: 
> the act of transforming ideas into words is an amazingly efficient way to solidify and refine your thoughts about a given topic. 

One great expectation I have for myself is that through the daily blogging, I will be able to thoroughly examine my understanding of concepts. Consequently, the writing should be coherent, clear, and simple because when you think about it even a complex idea/concept is a composition of underlying fundamental concepts which can be broken down and explained in a straight-forward manner.

Thus, it is essential for me to have a strong foundation in whatever domain of study I choose to pursue, or else it will be a constant struggle of trying to describe concepts in a convoluted, jargon-filled way *(not that there is anything wrong with using jargon but one of my goals it to try to **ELI5** - explain it like I'm five when it comes to what I have learned)*.     

## Today's Tasks

1. Taking care of the first order of business, I worked through the new hire paperwork and submitted all the required documents. 
2. Next, Micah provided me several links to help me create my first blogging site. I read through an [article on using Jekyll and GitHub Pages to build a blog](https://www.smashingmagazine.com/2014/08/build-blog-jekyll-github-pages/) and followed the brief tutorial on that article to build my blog, which you are reading right now. The other links were examples of other people's blogs that I found to be helpful and guided me in terms of what sort of content I should be posting on my blog. 
3. **Clojure Koans**. A *koan* is a riddle or a puzzle used during meditation to help someone contemplate some greater truths/realities. There are **27** Koans and each Koan is comprised of a number of exercises. The Clojure Docs came in clutch a couple of times when I found myself meditating a bit too long on a particular koan exercise. Also, I think this is an *excellent* way of learning the basics of Clojure and I am thoroughly enjoying myself. 

## TIL - Today I Learned...

### Clojure
* According to the [docs](https://clojuredocs.org/clojure.core/symbol)`(symbol name)` the `name` of the symbol can be *a string or a symbol, e.g. `symbol 'foo` or `symbol "foo"`*
* `Clojure.core` is a **namespace** and is Clojure's standard library. In OO languages where behavior is grouped **using classes**, *Clojure* uses **namespaces** to group similar behavior and state. 

### intelliJ/linux
* When I was cloning the Clojure Koan repo I ran into this error: ```Warning: Permanently added 'github.com,140.82.113.3' (RSA) to the list of known hosts.
git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository.``` I received this error because I was running on linux mint instead of my usual windows and because of that I did not have an existing ssh key for my linux mint. So, with the help of Micah, I found [an article on generating a new SSH and adding it to the ssh-agent](https://docs.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) and after generating a new ssh key, I used the `cat` command to view the contents of the public key, which I copied and saved into my github profile's ssh keys. 
* Using the `locate` command to find the path for `idea.sh` *(the file that is used to launch intelliJ).* A **SH file** is a simple text file that contains commands and some logic. In some ways, it is very similar to a *batch file* for Windows. In my case, the `.sh` file was ran on linux mint. 
* Created a *command line lanucher* for intelliJ. Now, I don't have to worry about finding where the idea.sh file is located. Also, the command line launcher conveniently allows me to launch intelliJ with the `idea` command. So, I went to `/home/gosupark/Projects/clojure-koans` and typed in the command `idea project.clj` to open up the **Clojure Koans** project and it worked like a charm. I love it when I discover ways to save time & streamline mundane tasks. 

## What's Next? 
- One ultimate goal is to work through all 27 Clojure Koans. (Figure out a good schedule & pace for this)
- I found this pretty in-depth [tutorial on Clojure](https://www.youtube.com/watch?v=zFPiPBIkAcQ&t=477s), so when I get the chance I would like to go through the entire video and probably take notes on it as well. 
- Continue to familiarize myself with linux mint & **the terminal**. (The terminal is a friend, not a foe)
- Try to work on the blog post throughout the day and as I face challenges or make breakthroughs I can write it into my blog. This will help me remember what happened throughout the day and keep the post more organized. 
- Clone this repo so I can blog locally in my favorite editor. 



