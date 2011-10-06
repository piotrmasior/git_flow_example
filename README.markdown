# Git flow live example

## How it works

Here is described original idea: http://nvie.com/posts/a-successful-git-branching-model/

About git flow itself you can read readme at github: https://github.com/nvie/gitflow there are some useful resources also

## Getting started

If you have got already cloned repository on your machine just run git flow init and press enter 7 times:

`git flow init`

` Which branch should be used for bringing forth production releases?
   - master

 Branch name for production releases: [master]

 Branch name for "next release" development: [develop]


 How to name your supporting branch prefixes?

 Feature branches? [feature/]

 Release branches? [release/]

 Hotfix branches? [hotfix/]

 Support branches? [support/]

 Version tag prefix? []`


`git branch --set-upstream develop origin/develop`

`git pull`

You are ready to start using it!

## By default

You are working by default on 'develop' branch. Here workflow is normal looks like this:


`touch some_file`

`echo "something" >> another_file`

`git add .`

`git commit -am 'some changes'`

`git pull`

if conflicts, solve them, commit

`git push`


## Use feature

When you have got some feature (for instance in tracker system)

 `git flow feature start 985`

985 is ticket number or whatever

do some work

 `git commit -m 'changed header'`

do more stuff

 `git commit -m 'changed footer'`

and when you decided that is completed

 `git flow feature finish 985`

you will be back at develop when everything goes fine where you can start new feature ;-)


## Share feature with others

Sometimes features are so big we need help, so we push our branch to repository to do this.
So first developer - call him A - will init this feature:

`git flow feature start 121`

`git flow feature publish 121`


now A and another developers:

`git flow feature track 121`


so now they all can start developing stuff, normally commit and push, commit push


after feature is done
`git flow feature finish 121`





# Current Version
  v0.2.0