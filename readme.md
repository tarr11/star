#Star#

## Overview ##
Star is a convention based json based file format for storing bookmarks.  You store your bookmarks in json files and put them whereever you want.

## Why? ##
I need a bookmarking tool.  I used to use Delicious.  Mostly I just use Ctrl-D in Chrome.  But all of this stuff is locked up proprietary data formats that I can't discover.

My vision is a world where I publish and own access to my data.  The value a company provides is providing an analysis of that data, not restricting access to it.  I can license it any way I wish as well, and companies should respect that license.

If a company wants to use it for their own purposes, fine, but they have to crawl it.  And I can remove it at any time.  But it's not stuck in some non-portable format and I can go somewhere else with it if things don't work out for that company.

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

Each file should contain one bookmark.  This allows us to use the file timestampes to determine when the bookmark was created.

## Folder Structure ##
Use the data directory to store all my bookmarks and notes.  Organize your files and folders under there however you want.  I'm personally starting with folders that are source (like /hackernews, /techcrunch, etc) and then folders that categorize those sources.  You could also organize by topic, date, or some othe r personal category; it doesn't really matter.

I'm not excited about a sitemap file format as it will just get out of data unless it is auto-generated.  And if it is auto-generated, it's not necessary here and can be done in some other tool.

## Bookmark creation ##
I'm not building any tools yet; I will soon.  The first thing I'd imagine is a Chrome based bookmarklet that dumps bookmarklets to Dropbox or Github based on the title and content of the page. 


## Utilities ##
I'll be storing any utilities at [star.util](https://github.com/tarr11/star.util) 
* Browser extensions, utility code, etc



