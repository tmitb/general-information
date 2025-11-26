# Welcome to tmitb repositories
This repository serves a purpose of the main gate of all other repositories in this account. Each repository has their our way of handling the specific requirements of it, however, there are common elements and generally accepted practices to them. This document serves the purpose of explaninig those common/general information that applies most, if not all, repositories.

## Parent and Children
There are repositories with a large topic which often houses smaller specific topics. For example, [home-automation](https://github.com/tmitb/home-automation) repo is the main repo that houses all things home automation, but there are sub modules that themselves have large enough scope. The way things are organized is normally as following

### Folder structure
/ (repo root)
- 'sub-module1 name'
- 'sub-module2 name'

It will never go down more than a level on its own, meaning that a sub module cannot have another sub module underneath.

### Naming convention
Repo names are following the rules below
- all the names are named using `Kebab case` unless it is impossible to use them for system restrictions, in which case, it will try `Snake case` and `Pascal case`
- sub-moudle repo must start with the parent module name. For example, a sub module for a home automation must start the `home-automation`. If the sub module name is *SD HVAC Controller*, the repo name will be `home-automation-sd-hvac-controller`
- where number of characters are limited, the name may be simply have a nickname. If even a nickname is too long, it will be named as `sub1` or even simply `1`

# License
Each repo has its own license, further, each folder or sub module of a repo can have its own license. This is due to the way projects are laid down. I could have everything in its own repo but I decided against that because that will be a disaster to manage.
