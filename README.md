# Git-SubTree-MainClassLibrary

> Git-SubTree-NetClassLibrary1
>
> ```cmd
> git remote add -f Git-SubTree-NetClassLibrary1 https://github.com/AhsenBaig-boilerplate/Git-SubTree-NetClassLibrary1.git
> git merge -s ours --no-commit --allow-unrelated-histories Git-SubTree-NetClassLibrary1/main
> git read-tree --prefix=Git-SubTree-NetClassLibrary1/ -u Git-SubTree-NetClassLibrary1/main
> git commit -m "Subtree merged in Git-SubTree-NetClassLibrary1"
> git pull -s subtree Git-SubTree-NetClassLibrary1 main
> git merge -X subtree=Git-SubTree-NetClassLibrary1 Git-SubTree-NetClassLibrary1/main
> git subtree pull --prefix=Git-SubTree-NetClassLibrary1 Git-SubTree-NetClassLibrary1 main
> git subtree push --prefix=Git-SubTree-NetClassLibrary1/ Git-SubTree-NetClassLibrary1 main -f
> ```

> Git-SubTree-NetClassLibrary2
>
> ```cmd
> git remote add -f Git-SubTree-NetClassLibrary2 https://github.com/AhsenBaig-boilerplate/Git-SubTree-NetClassLibrary2.git
> git merge -s ours --no-commit --allow-unrelated-histories Git-SubTree-NetClassLibrary2/main
> git read-tree --prefix=Git-SubTree-NetClassLibrary2/ -u Git-SubTree-NetClassLibrary2/main
> git commit -m "Subtree merged in Git-SubTree-NetClassLibrary2"
> git pull -s subtree Git-SubTree-NetClassLibrary2 main
> ```


# Subtree split example

> Split the source to subtree
> ```cmd
> git subtree split --prefix SubTree-NetClassLibrary3 -b split --rejoin --squash
> ```

> Push the split (create an empty repo for it on github)
> ```cmd
> git push https://github.com/AhsenBaig-boilerplate/Git-SubTree-NetClassLibrary3 split:main
> ```

## Sync subtree

> Pull
> ```cmd
> git subtree pull --prefix Git-SubTree-NetClassLibrary3 https://github.com/AhsenBaig-boilerplate/Git-SubTree-NetClassLibrary3 --squash
> ```

> Push
> ```cmd
> git subtree push --prefix Git-SubTree-NetClassLibrary3 https://github.com/AhsenBaig-boilerplate/Git-SubTree-NetClassLibrary3 --rejoin --squash
> ```
