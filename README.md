# Editing SheffieldUQ pages

These are the webpages for the SheffieldUQ group.

### Getting started

* Tell me your github name so that I can add you to the SheffUQ group.
* Clone the page
```
git clone https://github.com/rich-d-wilkinson/SheffUQwebpages
cd SheffUQwebpages
```


### Making changes etc.

The structure of the website is defined in /\_includes and /\_layouts.
The site is setup to use markdown. Content lives in .markdown or .md files, such as index.md. These are markdown files, so you don't need to use html tags (see [here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) for example).

Once you've made edits, you'll need to

* Run `jekyll serve --future TRUE` (You must install [jekyll](http://jekyllrb.com/) first).
* Open web browser and enter "http://127.0.0.1:4000/" to see the website.

If that looks okay, commit the code to github,

```
git add .  # or better, just add the files you've changed
git commit -m 'Description of changes'
git push --set-upstream origin master
```

 and upload it to cpanel.
The html files are those in the  /\_site directory.

```
cd _site
ftp username@staff.shef.ac.uk
# enter password
cd public_html
send index.html # I'll figure out how to do this in one go later.
```


### Blog entries

All blog post entries are stored in \_posts. The files must

* Create a new file that obeys the naming convention YEAR-MONTH-DATE-NAME.markdown
* You can use [markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet). I haven't sorted adding latex math equations yet, but I don't think that's hard.
* Include YAML header information such as
```
---
layout: post
title:  "event entry"
date:   2016-01-14
author: Richard Wilkinson
authorurl: http://r-wilkinson.staff.shef.ac.uk
categories: jekyll update events blog
---
```

* If you include the word 'blog' in the category keywords it will be listed in the blog entries, and if you include the word 'events', it will be on the events page etc.

* Note that events and blog entries in the future are not included by default, and so you need to specify that they should be included when you build the page:
```
jekyll serve --future TRUE
```

### Source
The website uses the [Jekyll-Pithy](https://github.com/smallmuou/Jekyll-Pithy) theme.
# RSS-Environmental.github.io
# RSS-Environmental.github.io
