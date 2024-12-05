# git-rebase-playground

## Using the editor

`git config --global sequence.editor "code --wait --reuse-window"`
`git -c sequence.editor="code --wait --reuse-window" rebase --interactive <commit>`
`git rebase -i <commit>^`  
  the caret means, not this commit but the one before.
`git rebase -i --root`
  `--root` means starting from the first commit.

## Edit a commit

use the `edit` keyword in the todo to modify a commit. You have to stage files and amend the commit.

## Untrack a file

`git rm -r --cached <file>` 
  `--cached` means we do not delete the file.

## Reword a commit message

use the `reword` keyword in the todo to reword the commit message of the commit.

## Drop a commit

use the `drop` keyword in the todo to get rid of a commit.

## Squash a commit

use the `squash` keyword in the todo to squash the commit into the previous commit.

## Insert a commit

use the `break` keyword in the todo between two commits to stop at a given commit and create a new commit here.

## Reorder commits

Just reorder the commits in the todo.

## Exec a command

use the `exec` keyword in the todo after a commit to with a command to exec.
`echo "Hello World"`
