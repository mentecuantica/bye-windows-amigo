# 2git 2gether

Well for me GIT as control version system is as simple as complex and powerfull.
May be the terminology - some words seems unfamiliar for me, for sure russian is my native, and yet i think Linus Torvalds had his own presentation.
Yep it seems actually easy to start using GIT, but using it righteous and in the team - for me it's not so obvious.
 

## Cleaning the mess in branches

----------

> My project on bitbucket origin repo is full of branches - of all types - deleted, obsolete , but on local MASTER repo i don't have them for long time... i don't need them 

#### I (and may be you too) forgot about PRUNE



cleanup

    
git gc --prune=now





**prune**

git remote prune public

       prune
       Deletes all stale tracking branches under <name>. These stale branches have already been removed from
       the remote repository referenced by <name>, but are still locally available in "remotes/<name>".
    
       With --dry-run option, report what branches will be pruned, but do no actually prune them.


**rm**

    git remote rm public 
    
       rm
       Remove the remote named <name>. All remote tracking branches and configuration settings for the remote
       are removed.


**fetch**

    > git fetch -p
> 
> It'll remove all your local branches which are remotely deleted.
> 
> If you are on git 1.8.5+ you can set this automatically
> 
> `git config fetch.prune true`
> 
> or
> 
> `git config --global fetch.prune true`


##LINKS

http://railsware.com/blog/2014/08/11/git-housekeeping-tutorial-clean-up-outdated-branches-in-local-and-remote-repositories/

http://blog.thefrontiergroup.com.au/2012/07/git-basics-cleaning-up-excess-branches/

http://www.gitguys.com/topics/adding-and-removing-remote-branches/


[http://stackoverflow.com/questions/4040717/git-remote-prune-didnt-show-as-many-pruned-branches-as-i-expected](http://stackoverflow.com/questions/4040717/git-remote-prune-didnt-show-as-many-pruned-branches-as-i-expected "git remote prune – didn't show as many pruned branches as I expected")