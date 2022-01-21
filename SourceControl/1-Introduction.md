# Source control


## What is it?

It is like a bank for your code. If you are familiar with Version control in documents (ie Word), then this is very similar, the only difference is that it's a family of documents rather than just the one.

> What is code? a.k.a: **source code** 
>
> An excellent question. Strictly one could say it's the text that when compiled or interpreted makes software. However,  you could say many things are code that we don't source control. 
>
>In this context, the answer is that code is all the text artifacts that need to be deployed to enable your business.

Source control is about coordinate the collaboration between multiple people.  How? 

* Knowing what changed when and if good practices are followed, why.
* Who changed it so that we can understand the context of the change when it is not clear.
* Associate some metadata to the change, for example when fixing a bug we can attach a ticket number or similar.
* As the owner of a repository you can control who has access to it.

Once you have some code, you need to do something with it so that it becomes useful. If this is a website, when the code changes it needs some process for the website to be updated, this process is called **Deployment**.


# Why is this useful, can't I just Dropbox, google drive, etc?

You might wonder why not use a simpler tool for sharing these text files, such as Dropbox, google drive, etc.

Dropbox and other remote storage solutions are great for some things, but if you are trying to store code, very soon you will need source control. 

Why?  It gets really painful when things are moving faster, especially if you loose the "right" version of it due to file naming like:


final.bak

final_do_not_delete.bak

final_do_not_delete(1).bak

final_do_not_delete(2).bak

ThisOne.bak
