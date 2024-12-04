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
