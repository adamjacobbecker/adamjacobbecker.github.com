---
layout: post
title: Be your own code review
---

The first time I used version control, (far less long ago than I'd care to admit,) I was introduced to the concept of peer code reviews. Before we'd commit something to our SVN repository, we'd generate a diff of our changes and post it up on RBCommons, and only once it was reviewed by another developer would it go into the repo. Now fast forward to the present -- I (and everyone I know) use git religiously, and the thought of using Subversion again makes me cringe. But when quickly iterating on a product, especially with only one other team member actively committing code, sometimes it's a lot easier to work right off the master branch instead of creating feature branches and pull requests for each minor tweak. And since this means that on occasion, the code I write doesn't get looked over by another developer before hitting production, I've implemented a little practice that I'm calling "self code review".

![github diff](http://i.imgur.com/0jcb7.png)

Yeah, I'm embarassed too that I call myself a developer and yet I'm still using Github for Mac, which one Stack Overflow user aptly dubbed "[Hasbro™ My Little Pony® Baby's First Git Client](http://stackoverflow.com/questions/455698/best-visual-client-for-git-on-mac-os-x)". But I swear, the fact that it shows me a beautiful, easy-to-read diff of my working tree makes my commits 100% better than if I just committed right after getting my code working. Even better, it lets me go file-by-file and split my commit into multiple smaller ones, if say, I fix one tiny issue as part of a bigger fix for another. And even if you're a die-hard command line user, you can just do a quick `git diff HEAD --color-words` and achieve practically the same result:

![CLI diff](http://i.imgur.com/jceDK.png)

These "self code reviews" aren't just a chance for me to make trivial changes like cleaning up my formatting or making sure my variable names make sense, but they're also a chance to take a breather, go back, and refactor my code before committing. But even if you know that someone else will be reviewing your code, at least take a second and make sure that person won't have to go around removing dummy variables or uncommenting lines that you only had intended to comment out temporarily, all because you were too quick to hit that commit button.