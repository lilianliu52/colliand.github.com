# J. Colliander's Web Site

## Deploy notes

I moved the .git folder from the top level directory into the subdirectory _site/.

Git commands should be executed from the terminal line within _site/.

Executing git from _site/ ensures that the locally generated version of the site is pushed to Github for hosting using Pages.

Why do this?

This site uses the [jekyll-scholar](https://github.com/inukshuk/jekyll-scholar) plugin to render the [bibliography](http://colliand.com/research/). Github pages processes jekyll sites witht the --safe flag toggled so plugins are not allowed. 