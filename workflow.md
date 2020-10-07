Generally, merge process proceeds in the order of this : feature -> develop -> release -> master (hotfix branch is used as an exception)
First, a new feature is developed by creating a new 'feature' branch. It must be came from the develop branch, not the master branch.
And when the feature development is done, It must be merged with the develop branch again. Be careful not to merge with the master branch.
Finally, QA will be proceeded in the release branch. And if there is no problem, the release branch will be is merged into the master branch and the develop branch, respectively, to finish the one version.
