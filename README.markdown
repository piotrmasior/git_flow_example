# Git flow live example

## How it works

Here is described original idea: http://nvie.com/posts/a-successful-git-branching-model/
About git flow itself you can read readme at github: https://github.com/nvie/gitflow there are some useful resources also

## Getting started

I don't like read too much so I created cheat sheet for every day use

If you have got already cloned repository on your machine just run git flow init and press enter 7 times:

`$ git flow init`

Which branch should be used for bringing forth production releases?
   - master
Branch name for production releases: [master]
Branch name for "next release" development: [develop]

How to name your supporting branch prefixes?
Feature branches? [feature/]
Release branches? [release/]
Hotfix branches? [hotfix/]
Support branches? [support/]
Version tag prefix? []

`$ git branch --set-upstream develop origin/develop`
and finally
`$ git pull`

and you are ready to start using it

## By default

You are working by default on 'develop' branch. Here workflow is normal looks like this:

`$ git pull`
`$ touch some_file`
`$ echo "something" >> another_file`
`$ git add .`
`$ git commit -am 'some changes'`
`$ git push`






# Current Version
  v0.1.0