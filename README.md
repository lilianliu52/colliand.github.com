colliand.github.com
===================

James Colliander's web pages repository


Deploy notes:
from source directory
> git commit, push, add, etc.
> bundle exec jekyll build

That will copy all the files into the built directory
from the built directory
> git commit -A,  add, etc.
> git push to move the files to github.io master branch to populate CNAME.com

[Martin Muñoz wrote a gist for me.](https://gist.github.com/mmun/5d660193f89df8de6efa)

cd ~/colliand-source
 
# Commit & push your source. Not necessary but a good idea.
git add -A
git commit -m "Made some updates"
git push
 
# Build the blog to the ~/colliand-built folder
bundle exec jekyll build
 
# Switch to ~/colliand-built, commit and push.
# GitHub Pages will deploy the website automatically
cd ~/colliand-built
git add -A
git commit -m "Publish"
git push