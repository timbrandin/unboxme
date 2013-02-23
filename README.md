## Unboxing

`curl http://github.com/unboxme/unboxme.sh | sh`

Setup of ~/boxes and installs dependencies (Vagrant, VirtualBox, Git, etc).

## Create new project

`unboxme __PROJECT__ [__SAMPLE__]`

Samples is also listed here: http://github.com/unboxme/packages

## Create project out of existing source

`unboxme __FOLDER__`

## Build / Re-build

`unboxme [__PROJECT__] build [__BRANCH__]`

## Install / Re-install

`unboxme [__PROJECT__] install`

## Stage

`unboxme [__PROJECT__] stage [__LOCATION__]`

## Deploy

`unboxme [__PROJECT__] deploy [__LOCATION__]`

## Navigate / Switch to a project from anywhere

`unboxme __PROJECT__`

* Terminates any other current running project and initates __PROJECT__.
* Will also set the title of the terminal to read __PROJECT__ in uppercase. 

## Add package

`unboxme [__PROJECT__] add __PACKAGE__`

Packages is also listed here: http://github.com/unboxme/packages.

## Destroy project

`unboxme [__PROJECT__] destroy`

## Upgrade unboxes

`unboxme upgrade`

## Uninstall unboxes

`unboxme unistall`

## Install extenstions

`unboxme install __EXTENSION__`

Extensions is also listed here: http://github.com/unboxme/extenstions.

# Manual

`unboxme man`
