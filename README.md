# test-revert

Test Git for `git-revert`!

### Undo a "public" change

Scenario: You just ran `git push`, sending your changes to GitHub, now you realize there's a problem with one of those commits. You'd like to undo that commit.

Undo with: `git revert <SHA>`

What's happening: `git revert` will create a new commit that's the opposite (or inverse) of the given SHA. If the old commit is "matter", the new commit is "anti-matter"—anything removed in the old commit will be added in the new commit and anything added in the old commit will be removed in the new commit.

This is Git's safest, most basic "undo" scenario, because it doesn't alter history—so you can now `git push` the new "inverse" commit to undo your mistaken commit.