# 666b FORUM

I wrote the code for this "forum" after reading [A Fully Function PHP
Forum in 964 Bytes of
Code](http://www.nerdparadise.com/tech/php/1kbforum/), thinking that
it would be interesting to see if I could add more features to the
forum while reducing the code size even further. The forum is mostly
based on that original idea and code.

This forum might not work in all web browsers since the HTML
is purposefully invalid. I have only tested it with Firefox and
Chromium.

## Features

* Anyone can start a topic and write a first post under the thread
* Anyone can reply to any thread
* Removes extra whitespace and doesn't allow empty posts
* Limits the posts to at most 999 characters
* Making use of PDO for database abstraction
* The SQLite database is automatically created initially
* Protected against XSS exploits
* Protected against SQL injections
* Exploits PHP and HTML to make the code really compact

## Requirements

* A web server with PHP 5 and SQLite.
* The web server must have write access to the forum's directory.
* Magic quotes should be turned off.
