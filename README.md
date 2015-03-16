# Bible API
===========

[Demo Bible API](https://guarded-beyond-9967.herokuapp.com/)

Create your own Bible API using Sinatra (Sinatra is a DSL for quickly creating web applications in Ruby with minimal effort)

> No database required! The whole Bible are on static files (`/public` in *JSON* format)

## Installation
---------------

* Install Sinatra `$ gem install sinatra`
* Install Thin web server `$ gem install thin`
* Install Json `$ gem install json`
* Type `$ ruby index.rb` to start the server
* Go to `http://localhost:4567` in your browser


## Usage
----------
Get All Books

    http://localhost:4567/api

Get Chapters from Book

    http://localhost:4567/api/:bookname
    eg.: http://localhost:4567/api/Genesis

Get Verses from Chapter

    http://localhost:4567/api/:bookname/:chapter
    eg.: http://localhost:4567/api/Genesis/1

Get single Verse

    http://localhost:4567/api/:bookname/:chapter/:verse
    eg.: http://localhost:4567/api/Genesis/1/3