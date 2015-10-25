---
layout: page
title: Portfolio
permalink: /portfolio/
---

This is a showcase of some of my projects that I have done, and am working on.

Most of them are school projects, things I have done for different courses at school. As such they have pretty limited scope and may contain bugs, something to expect when the projects lasted for around 2 weeks each.

Most things I have done can be found at my [Github](https://github.com/CCHolmgren).

## Showcase

### Restaurant list
![](/images/ss+2015-10-25+at+02.07.36.jpg)
[Restaurant list](http://django.christofferholmgren.se/) is a page to find and explore restaurants. It's difficult to find new ones, tiresome to search for them, and which ones have you visited? These are the problems that Restaurant List tries to alleviate.

Languages: **Python**, **JavaScript**, other techniques: **Django**, **jQuery**.

### PHPForms
![](/images/ss+2015-04-30+at+03.41.48.png)
[PHPForms](https://github.com/CCHolmgren/PHPForms) is a library for creating and handling forms using nothing but PHP 5.4+.
The library tries to be feature complete with Laravel-form-builder, a library for PHP forms that has a dependency to Laravel, while at the same time not depend on it itself.
I also wanted some features that are inspired from Django, such as the formatting of forms using ```to_p```, ```to_ul```, ```to_table``` functions. It has a ```asDivs``` method that allows you to format your form as divs, but you may also format it any way you please with a little less terse API.
It also provides validators and allows you to easily create new ones, or use some built in ones if you please.
The main goal was the compatibility with Laravel-form-builder, but also to have a modular system, so that as many parts as possible are extendable if you want some feature that is missing.  

Languages: **PHP**, other techniques: **composer**

* * *

## Projects done while studying at Linneaus University

# Projects TOC
* [Music Comparer](#music-comparer)
* [Kubus](#kubus)
* [Quiz-a-tron](#quiz-a-tron) 
* [Ruby on Rails and AngularJS project](#ruby-on-rails-and-angularjs-project)
* [Forum/bookmark site](#forumbookmark-site)
* [1DV449](#dv449)  
    1. [Laboration 1 and 2](#laboration-1-and-laboration-2-in-1dv449)

* * *

### Music Comparer
![](/images/ss+2015-04-30+at+12.32.27.png)
[Music Comparer](http://node.christofferholmgren.se/) is a page that gathers information from Last.FM and Spotify and compares artists with eachother. There was also an added requirement of it being offline-first, so Music Comparer caches searches to enable comparisons whilst offline.   
The task that we were given was to develop an application that uses at least two different API's, and also uses OAuth in some part of the application.  
Because my application doesn't rely on the OAuth part at all I used the Last.FM login API to prevent using the application without signing in. And as you can see, you will be redirected to the base url (```http://node.christofferholmgren.se/```) if you try to access the ```/application``` url without signing in. This will most likely get changed when I have time.  
The backend runs Node.js and uses Redis with RDB enabled as a persistent in-memory database. 
Due to the lacking LocalStorage API that browsers provide there is no way to TTL mark the caching without using some library to provide this functionality, and as such the searches will not be updated. This shouldn't affect things, but it might hinder some things if more development is done.
Code can be found [here](https://github.com/CCHolmgren/Music-comparer).   
Languages: **Javascript**, other techniques: **NodeJS**, **express**, **redis**  

### Kubus
![](/images/ss+2015-05-04+at+02.29.46.jpg)
[Kubus](http://www2.kau.se/jorrbomm/) is a project developed in a team. Kubus is a cube builder application intended to be used on iPads and other mobile units, but can also be used on your computer without any problem. It uses ThreeJS and jQuery with a PHP backend.
This project involved all parts of a larger project. Meetings with the customer, desigining the application, risks, testing and so on. In the end we delivered an application that is focused on math education for school classes in the ages 7-12 years.
Languages: **Javascript**, **PHP**, other techniques: **ThreeJS**, **jQuery**, **SCRUM**, **Teamwork**, **Responsive**

### Quiz-a-tron
![](/images/ss+2015-04-30+at+12.42.24.png)
[Quiz-a-tron](http://www.christofferholmgren.se/quiz-a-tron/) is a quiz-making/-taking page.  
The backend runs PHP 5.4 and uses PostgreSQL as the database.
Code can be found [here](https://github.com/CCHolmgren/Quiz-a-tron).
Languages: **PHP**, other techniques: **PostgreSQL**, **Bootstrap**

### Ruby on Rails and AngularJS project
[Ruby on Rails and AngularJS project](https://github.com/CCHolmgren/ch222kv_1dv450_kod). Ruby on Rails on the backend that provides the API. AngularJS to handle the frontend with everything that is involved in that. A PostgreSQL was used to develop it, but because the peer reviewer couldn't get PostgreSQL setup, I switched it out for SQLite instead. This meant breaking the search functionality, but it was a small price to pay.
Languages: **Ruby**, **Javascript**, other techniques: **AngularJS**, **Ruby on Rails**, **PostgreSQL**, **SQLite**

### Forum/bookmark site
[Flask and SQLAlchemy Python project](https://github.com/CCHolmgren/individuellt_mjukvaruprojekt). I looked at my bookmarks and saw that it isn't particularly easy to share bookmarks, and this service was born. The idea is that you savce your links in collections and then you can share these collections with anybody that you want easily. The project also includes a forum. Uses Python and Flask for the webservice and SQLAlchemy as the ORM. Markdown is used in the forum and in the collections to provide styling and such without security problems.  
Languages: **Python**, other techniques: **Flask**, **SQLAlchemy**

## 1DV449
[Webbteknik II](http://coursepress.lnu.se/kurs/webbteknik-ii/)  

>Kursen Webbteknik II vid Linnéuniversitetet
>
>Denna kurs fokuserar helt på webben. Kursen tar upp webbens historia, utveckling och betydelse för samhället, problem inom forskningen kring webben (Web Science). Kursen tar också upp optimering och säkerhet i webbapplikationer. Stort fokus kommer att ligga i att kunna hantera öppna Webb-API:er för att sammanfoga data i så kallade mashup-applikationer.

All in all a course focused on the web, how to develop API's and how to consume those API's. We developed a mashup-application, and my is called [Music Comparer](#music-comparer). We also did two smaller practical tasks.  

### Laboration 1 and Laboration 2 in 1DV449
[1DV449](https://github.com/CCHolmgren/1DV449_ch222kv)
The first task was to develop a web scraper and scrape the coursepress.lnu.se page for courses. I did this using PHP and libcurl. And the code can be found [here](https://github.com/CCHolmgren/1DV449_ch222kv/tree/master/Laboration-1).
Languages: **PHP**
The next task was to take some bad code and make it better. Improve the security of it, optimize the loadtime of the page and also implement a simple long polling functionality to provide a simple chat. The code can be found [here](https://github.com/CCHolmgren/1DV449_ch222kv/tree/master/Laboration-2) with all the notes of changes that I did. 

The last task was to do a mashup-application, which you can find above in the [showcase](#music-comparer).