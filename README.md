# Editing SheffieldUQ pages

These are the webpages for the Royal Statistical Society Environmental Statistics Section.

### Getting started

* Request to joint the RSS-Environmental organisation on github (email me  your github id)
* Clone the page
```
git clone https://github.com/RSS-Environmental/RSS-Environmental.github.io.git
cd RSS-Environmental
```
###

### Making changes etc.


The site uses [markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)  to create pages using [jekyll](http://jekyllrb.com/). Hence there is no need to use or know any html. Content lives in .markdown or .md files, such as index.md.


The structure of the website is defined in /\_includes and /\_layouts.

Once you've made edits, you'll need to

* Run `jekyll serve` (You must install [jekyll](http://jekyllrb.com/) first) to check you are happy with your changes (enter "http://127.0.0.1:4000/" in a web browser to see the website)

* If that looks okay, commit the changes and push to github.


### Blog entries

All blog post entries are stored in \_posts. The files must

* Create a new file that obeys the naming convention YEAR-MONTH-DATE-NAME.markdown
* You can use [markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).
* Include YAML header information such as
```
---
layout: post
title:  "event entry"
date:   2016-01-14
author: Richard Wilkinson
authorurl: http://r-wilkinson.staff.shef.ac.uk
categories: jekyll update events
---
```

* Note that events are automatically sorted into future and past events according to the date. However, the date is set when the website is built, so to move events to being past events, the website needs rebuilding (make a small change, e.g. add a meeting report, and push it back to github).

### Committee membership

Committee member details are stored in
```_data/members.yml ```
as a list. Update the information here with your webpage etc.


### Source
The website uses the [Jekyll-Pithy](https://github.com/smallmuou/Jekyll-Pithy) theme.
