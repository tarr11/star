#Star#

## Overview ##
Star is a convention based json based file format for storing bookmarks.  You store your bookmarks in json files and put them whereever you want.

## Why? ##
I need a bookmarking tool.  I used to use Delicious.  Mostly I just use Ctrl-D in Chrome.  But all of this stuff is locked up proprietary data formats that I can't discover.

My vision is a world where I publish and own access to my data.  If you want to use it for your own nefarious purposes, fine, but you have to crawl it.  And I can remove it at any time.

I also prefer to have my primary source of data be in files and folders.  I just like that better.  

* I can edit them in my favorite text editors (vim, sublime text, visual studio)
* I can publish and unpublish at my whim to websites, dropbox, github, or anywhere else that supports files
* I am not constrained to a relational db schema.

## File Structure ##
I'm using json to store the data.  I like json because:

* It's fairly human-readable and editable (but not perfectly)
* It's easy to parse in just about any modern programming language.
* It doesn't have a fixed schema and lets me add whatever I want to it.

It's going to be pretty loosely conventional.  Fields like website, comment, etc, but that are mostly focused on readability.  I'm not excited about sticking non-human-readable things like UUIDs, timestamps, or GUIDs in this structure.

## Folder Structure ##
Use the data directory to store all my bookmarks and notes.  Organize your files and folders under there however you want.  I'm personally starting with files that are source (like hn=hackernews, tc=techcrunch, etc) and then folders that categorize those sources.

I'm not excited about a sitemap file format as it will just get out of data unless it is auto-generated.  And if it is auto-generated, it's not necessary here and can be done in some other tool.

Use the src directory for utilities in various languages and tools.  Eventually, I'll move that out into a separate project I guess.

## Utilities ##
[star.util](https://github.com/tarr11/star.util) 
* Browser extensions, utilitiy code, etc



