Knowledge Check

- How can you amend your last commit?

- What are some different ways to rewrite history?

- What is a safe way to push history changes to a rempote repository

- What are the DANGERS of history-changing operations

- What are the BEST practices of history-changing operations

- Explain what it means for branches to be pointers.
  "Branches - is a way to keep multiple different versions of the same project or file but under the hood, a branch is a pointer to a single commit! Each commit is also a pointer."
  "Pointers - are used to point to the commit previously to it. Just like a linked lis

<!-- Changing History -->

Changing The Last Commit

(!) --amend : Lets you modify your last commit. You can change your log files that appear in the commit.
(Did you make a typo? Add something ny accident? This is when you'd use -ammend)

REMEMBER to only amend commits that have not been pushed anywhere!

Changing Multiple Commits

rebase -i : allows us to interactivly stop after each commit we're trying to modify, and then make whatever changes we wish. We do have to tellt his command which is the last commit we want to edit like so...

git rebase -i HEAD~2 : allows us to edit the last two commits. If we want to edit one of these commits, we'd change the word 'pick' to 'edit'

squash : is a handy way of keeping our Git history tidy. It's important to know how to squash because this process may be the standard on some development teams.

Splitting Up a Commit

reset : is the reverse of squash, instead of combining two commits, you van split a commit in two (All of these edits are using rebase to sift through which commits to edit.) Running reset resets the branch and updates the index (staging area).

Branches are Pointers!
