# git-delta-tree

Given a `diff-tree` style range creates a new tree object that contain only the
changed files.

    git-delta-tree HEAD~4..HEAD

A neat thing you can do with this is create a tarball of the changes

    git archive `git-delta-tree HEAD~4..HEAD` -o patch.tgz
