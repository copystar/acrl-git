<!---
This article is CC0, aka the public domain, aka do what you want with it. Full text of the Creative Commons CC0 license can be found here: http://creativecommons.org/publicdomain/zero/1.0/legalcode
-->

An Introduction To Modern Version Control That Will Quite Possibly Leave You Feeling More Confused Than When You Started
==========


What if I told you there was something very much like Dropbox but had a difficult learning curve? Something that, rather than being easy to install and use, actually required a not-insignificant time investment to learn? And that rather than operating automatically, required you to execute a number of steps *beyond* hitting save in Word? Would you ask me why I'm telling you about this?

Writing software is hard business -- don't believe anyone who puts forward the front that they can birth fully-functioning code apropos of nothing. Programming is *iterative*; you write something, you test it, it breaks, you fix it, you write some more, it breaks something else. And it's a common scenario to have a bug arise in your code that you wrote ages ago, sometimes years ago, and you need to go back to how your code looked at a specific point in time to fix it. Common also is adding features to already mature code; features that may break existing functionality, features that need some working out to actually function, and you want to keep them separate from what's already working.

Enter version control. In programming, a *version control system* is a program that, at a very basic level, records the state of a project and has functionality to view past states, commonly called a *repository* and allows people to collaborate on that repository. Modern version control systems have the ability to incorporate changes to that state from multiple contributors, keep all revisions of a project indefinitely, have as many backups as the project as there are people with copies of the repository, and make it easy to collaborate with others. For simple projects it might be overkill, but when you're dealing with million-line codebases with hundreds to thousands of contributors, a system that keeps track of who did what when makes administration of a project not easier, but *possible*.  Version control's been around a number of years, and there have been [a number of implementations](http://en.wikipedia.org/wiki/List_of_revision_control_software) of it, but modern version control systems break down into basically two camps: *decentralized* (or distributed) version control and *centralized* version control (and, like most things in the software world, into *proprietary* and *open source* as well).

Dropbox, mentioned earlier, can be thought of as a version of centralized control. You have your client machine, it has a Dropbox folder, and that folder hooks up to Dropbox HQ. Dropbox HQ will always try to have the most up to date version of your Dropbox folder; if you log into Dropbox's web interface after moving a file into your local folder, you'll see that file there. If you have a friend you want to share a file with via Dropbox, that person also connects to Dropbox HQ to read the files. If your friend is absolutely unable to connect to Dropbox, they're not going to be able to read the files you put there as Dropbox is the *central repository* of your files. If you lose connectivity to Dropbox -- let's say if you're working on something on the airplane -- then your files aren't backed up until you get back on the network.

A lot of version control systems work like Dropbox. [Subversion](http://subversion.apache.org/) is the most popular one and it, like Dropbox, requires that you have a central place to put files. Unlike Dropbox, there is no single Subversion company that runs a repository; you can put a Subversion server on your own machine. But in other respects it is largely similar -- your friend again needs to be able to reach your Subversion server to be able to read your files. Having one *workflow* like this has a distinct advantage -- one workflow means one way of doing things and cuts down on confusion -- but the moment you have an unusual workflow you'll find yourself working against the system rather than with it.

If you're a serious Dropbox wonk, you've probably noticed that Dropbox keeps the last ten or so saves of each file -- handy if you nuke something and need to go back to an earlier revision. But if you're a compulsive saver, you'll quickly run out of those last ten revisions.  Any modern version control system will keep *every single revision* ever made to a project, so going back to any point in development is easy.

A decentralized version control system, like [git](http://git-scm.com), [Bazaar](http://bazaar.canonical.com), or [Mercurial](http://mercurial.selenic.com), doesn't need a central repository. A decentralized version control system can be run entirely locally, without sharing files at all, or it can be run in a manner similar to a centralized one. This [workflow flexibility](http://git-scm.com/book/en/Distributed-Git-Distributed-Workflows) 



(griffey gource youtube video link: http://www.youtube.com/watch?v=RbfL_g4mtcw)


 

