--- 
layout: post
title: "Transfer YouTube favourites and subscriptions between accounts"
author: "Mark"
comments: false
---

At one point I wanted to transfer my [YouTube](http://www.youtube.com "YouTube")
favourites and subscriptions from one account to another. I couldn't find an
application that would let me do that, so last year I wrote one of my own.

If you are looking to do the same and you're running Windows with .NET installed,
you can grab the application from the
[downloads](https://bitbucket.org/readysetmark/youtube-favourites-transfer/downloads "Bitbucket project downloads page")
page of the BitBucket [project](https://bitbucket.org/readysetmark/youtube-favourites-transfer/overview "Bitbucket project page").

It's a console application. When you run it, you'll be prompted for the login
and password for the YouTube account to export subscription and favourites data 
from. Once the data has been exported, you'll be prompted for the login and 
password for the YouTube account to import the data into. Then it'll notify you
when it's done!

Beware, the password will be shown in cleartext in the console prompt, so only
do this when you have some privacy. The YouTube API is accessed over HTTPS, so
your password and data are secure when transferred over the internet.

You're welcome to view the [source code](https://bitbucket.org/readysetmark/youtube-favourites-transfer/src "Bitbucket project source page"). The application was my first F# application, although the code is 
largely procedural. Note that if you want to compile and run it yourself, you'll
need to get and supply your own YouTube Developer Key. Look for the 
``devkey_token`` variable in the source code.