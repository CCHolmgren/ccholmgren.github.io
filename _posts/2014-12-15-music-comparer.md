---
title: "Node.js: Music Comparer"
---

![](/images/ss+2015-04-30+at+12.32.27.png)
Music Comparer is a page that gathers information from Last.FM and Spotify and compares artists with eachother. There was also an added requirement of it being offline-first, so Music Comparer caches searches to enable comparisons whilst offline.   
The task that we were given was to develop an application that uses at least two different API's, and also uses OAuth in some part of the application.  
Because my application doesn't rely on the OAuth part at all I used the Last.FM login API to prevent using the application without signing in.
The backend runs Node.js and uses Redis with RDB enabled as a sort of  persistent in-memory database. 
Due to the lacking LocalStorage API that browsers provide there is no way to TTL mark the caching without using some library to provide this functionality, and as such the searches will not be updated. This shouldn't affect things, but it might hinder some things if more development is done.
Code can be found [here](https://github.com/CCHolmgren/Music-comparer).

Languages: **Javascript**, other techniques: **NodeJS**, **express**, **redis**  