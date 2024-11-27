# git-rebase-playground

## Using the editor

`git config --global sequence.editor "code --wait --reuse-window"`
`git -c sequence.editor="code --wait --reuse-window" rebase --interactive <commit>`
`git rebase -i <commit>^`  
  the caret means, not this commit but the one before.
`git rebase -i --root`
  `--root` means starting from the first commit.
