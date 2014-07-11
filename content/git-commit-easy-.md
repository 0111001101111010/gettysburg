title: git-commit easy 
date: 2014-02-05 19:52:17
tags:
---

Git's easy way to merge conflicts in pull requests

The suggestful cli prompts to the simplicity of github. 

``` shell
Step 1: From your project repository, check out a new branch and test the changes.
git checkout -b ajspeller-gh-pages gh-pages # on your branch 
git pull https://github.com/ajspeller/c4hrva-landing.git gh-pages
#should get a conflict 
Step 2: Merge the changes and update on GitHub.
git checkout gh-pages
git merge ajspeller-gh-pages
git push origin gh-pages
```


