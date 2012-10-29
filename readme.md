#Star.json#

## Overview ##
Star.json is a convention based json based file format for storing bookmarks.

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

## Folder Structure ##
Use the data directory to store all my bookmarks and notes.

Use the src directory for utilities in various languages and tools

## Roadmap ##
* First thing I need is a chrome extension so I can bookmark easily.
* Other stuff
 * vim plugin for editing star.json files easily
 * sublime-text (same)
* Some tool to publish changes automagically to git or github




