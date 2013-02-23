## Unboxing

`curl http://github.com/unboxme/unboxme.sh | sh`

Setup of ~/boxes and installs dependencies (Vagrant, VirtualBox, Git, etc).

## Create new project

`unboxme __PROJECT__ [__SAMPLE__]`

Short version: `ubx __PROJECT__ [__SAMPLE__]`

Samples is also listed here: http://github.com/unboxme/packages

## Create project out of existing source

`unboxme __FOLDER__`

Short version: `ubx __FOLDER__`

## Build / Re-build

`unboxme [__PROJECT__] build [__BRANCH__]`

Short version: `ubx [__PROJECT__] -b [__BRANCH__]`

## Install / Re-install

`unboxme [__PROJECT__] install [__LOCAL__]`

Short version: `ubx [__PROJECT__] -i [__LOCAL__]`

Installs the project and sets local project url to __LOCAL__.

## Add package

`unboxme [__PROJECT__] add __PACKAGE__`

Short version: `ubx [__PROJECT__] + __PACKAGE__`

Packages is also listed here: http://github.com/unboxme/packages.

## Stage

`unboxme [__PROJECT__] stage [__LOCATION__]`

Short version: `ubx [__PROJECT__] -s  [__LOCATION__]`

## Deploy

`unboxme [__PROJECT__] deploy [__LOCATION__]`

Short version: `ubx [__PROJECT__] -d [__LOCATION__]`

## Navigate / Switch to a project from anywhere

`unboxme __PROJECT__`

Short version: `ubx [__PROJECT__]`

* Terminates any other current running project and initates __PROJECT__.
* Will also set the title of the terminal to read __PROJECT__ in uppercase. 

## Destroy project

`unboxme [__PROJECT__] remove`

Short version: `ubx [__PROJECT__] destroy`

## Upgrade unboxme on your machine

`unboxme upgrade`

## Remove unboxme from your machine

`unboxme remove`

## Extend unboxme with extensions

`unboxme extend __EXTENSION__`

Extensions is also listed here: http://github.com/unboxme/extenstions.

## Queuing multiple commands examples

`unboxme backend-boys drupal-bootstrap stage`

1. Creates new project "backend-boys" from sample "drupal-bootstrap"
2. Builds and installs as usual with new projects
3. Stages project to for example: fingerstache-wolf.unbox.me

Short version: `ubx backend-boys drupal-bootstrap -s`

`unboxme backend-boys build install stage`

1. Navigates to project "backend-boys"
2. Builds the project
3. Installs the project
3. Stages project to for example: fingerstache-wolf.unbox.me

Short version: `ubx backend-boys -bis`

## Manual

`unboxme man`
