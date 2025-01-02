# TL;DR (Quick Steps):
# 1. git fetch upstream
# 2. git checkout master
# 3. git merge upstream/master
# 4. Resolve any conflicts: edit files, git add <resolved-file>, git commit
# 5. git push origin master

# Full Steps:

# Note: The "upstream" remote should already be configured for your repository.
#       This is typically done with:
#       git remote add upstream <upstream-repo-url>
#       If you're following these steps, you can skip this setup.

# 1. Fetch the latest changes from the upstream repository.
git fetch upstream

# 2. Switch to the branch you want to sync (e.g., master).
git checkout master

# 3. Merge the upstream branch into your local branch.
git merge upstream/master

#    - If there are no conflicts, the merge will complete automatically.
#    - If conflicts are detected, Git will pause the merge process and show a list of conflicted files.

# 4. Check the status of conflicted files.
git status

# 5. Open and resolve conflicts in the listed files using your preferred editor.
#    - Look for lines marked with conflict markers:
#        <<<<<<< HEAD
#        (your changes)
#        =======
#        (upstream changes)
#        >>>>>>> upstream/master
#    - Decide which changes to keep, remove the conflict markers, and save the file.

# 6. Mark resolved files as resolved.
git add <file-with-conflicts-resolved>

# 7. Complete the merge process.
git commit

# 8. Push the updated branch to your fork.
git push origin master

# 9. Verify that your fork is now synced with the upstream repository.
git diff upstream/master
# TL;DR (Quick Steps):
# 1. git fetch upstream
# 2. git checkout master
# 3. git merge upstream/master
# 4. Resolve any conflicts: edit files, git add <resolved-file>, git commit
# 5. git push origin master

# Full Steps:

# Note: The "upstream" remote should already be configured for your repository.
#       This is typically done with:
#       git remote add upstream <upstream-repo-url>
#       If you're following these steps, you can skip this setup.

# 1. Fetch the latest changes from the upstream repository.
git fetch upstream

# 2. Switch to the branch you want to sync (e.g., master).
git checkout master

# 3. Merge the upstream branch into your local branch.
git merge upstream/master

#    - If there are no conflicts, the merge will complete automatically.
#    - If conflicts are detected, Git will pause the merge process and show a list of conflicted files.

# 4. Check the status of conflicted files.
git status

# 5. Open and resolve conflicts in the listed files using your preferred editor.
#    - Look for lines marked with conflict markers:
#        <<<<<<< HEAD
#        (your changes)
#        =======
#        (upstream changes)
#        >>>>>>> upstream/master
#    - Decide which changes to keep, remove the conflict markers, and save the file.

# 6. Mark resolved files as resolved.
git add <file-with-conflicts-resolved>

# 7. Complete the merge process.
git commit

# 8. Push the updated branch to your fork.
git push origin master

# 9. Verify that your fork is now synced with the upstream repository.
git diff upstream/master

