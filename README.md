parent
======

[![Build Status](https://api.travis-ci.org/ivanceras/parent.svg)](https://travis-ci.org/ivanceras/parent)

parent for ORM, fluentsql and commons

This is only for unifying the version of the 3 maven projects associated with ivanceras orm

# releasing
Releasing is done using maven

From develop branch that you have been working on.
Checkout to master code then merge the development branch to master
Push the result of the merge to origin repository master branch


```sh

git status
   origin develop
git checkout master
git merge develop
git push -u origin master
mvn -P ossrh clean deploy release:prepare release:perform

```
After deployment
Go back to development branch, then merge the master to development

```sh

git status
    origin origin master
git checkout develop
git merge master

```

From there, you can now continue development.

