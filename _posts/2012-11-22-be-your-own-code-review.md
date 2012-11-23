---
layout: post
title: Be your own code review
---

The first time I used version control, far less long ago than I'd care to admit, I was introduced to the concept of peer code review. Before we'd commit something to our SVN repository, we'd first generate a diff of our changes and post it up on ________, and only once it was reviewed by another developer would it go into the repo. Now fast forward to the present -- I (and everyone I know) use git religiously, and the thought of using Subversion again literally makes me cringe. But when quickly iterating on a product, especially with only one other team member actively committing code, sometimes it's a lot easier to work right off the master branch instead of creating feature branches and pull requests for each minor tweak. And since this means that on occasion the code I write doesn't get looked over by another set of eyes before hitting production, I've implemented a little practice that I'm calling "self code review".

!()[] github diff

Yeah, I'm embarassed too that I call myself a developer and yet I'm using Github for Mac, which one apt Stack Overflow user described as "_____________". But I swear, the fact that it shows me a beautiful, easy-to-read diff of my working tree makes my commits 100% better than if I just committed right after getting my code working. Even better, it lets me go file-by-file and split my commit into multiple smaller ones, if say, I fix one tiny issue as part of a bigger fix for another. And even if you're a die-hard command line user, you can just do a quick `git diff --color-words`_____ and achieve practically the same result:

!()[] terminal diff

These "self code reviews" aren't just a chance for me to make trivial changes like cleaning up my formatting or making sure my variable names make sense, but it's also a chance to take a breather, go back, and maybe even refactor my code before committing. But even if you know someone else will be reviewing your code, at least take a second and make sure that person won't have to go around removing dummy variables or uncommenting lines that you intended to comment out temporarily, all because you were too quick to hit that commit button. After all, there's only so many times in my life that I care to see a `$yermom` variable sitting in a government codebase. (Sorry, Jed :P!)