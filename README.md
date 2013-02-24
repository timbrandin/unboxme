# An [imaginary] web development environment manager.

For both mac and unix.

### Requirements
* A __github__ account setup and working.
* [Homebrew](http://mxcl.github.com/homebrew/) on OSX.

### Features
* Virtualization
* Unboxing (Creation/Setup of a distribution).
* Building
* Installing
* Extending
* Versioning
* Staging
* Deployment
* It is always up to date!

## Getting started

* OSX: `brew install unboxme`
* Debian: `apt-get install unboxme`

Setup of ~/boxes and installs dependencies (Vagrant, VirtualBox, Git, Drush, etc).

## Create new project

`unboxme __PROJECT__ [__SAMPLE__]`

Short version: `nb __PROJECT__ [__SAMPLE__]`

Samples is also listed here: http://github.com/unboxme/samples

## Create project out of existing source

`unboxme [__FOLDER__]`

Short version: `nb [__FOLDER__]`

## Build / Re-build

`unboxme [__PROJECT__] [build [__BRANCH__]]`

Short version: `nb [__PROJECT__] -b [__BRANCH__]`

Default is master, btw master should always be deployable so keep your changes in branches.

## Install / Re-install

`unboxme [__PROJECT__] install [__LOCAL__]`

Short version: `nb [__PROJECT__] -i [__LOCAL__]`

Installs the project and sets local project url to __LOCAL__.

## Open project in browser

`unboxme [__PROJECT__] open`

Short version: `nb [__PROJECT__] -o`

## Add package

`unboxme [__PROJECT__] add __PACKAGE__`

Short version: `nb [__PROJECT__] +__PACKAGE__`

Packages is also listed here: http://github.com/unboxme/packages.

1. Downloads the package
2. The environment creates a dump of the database.
2. Enables and installs the package
3. Runs a database update if needed.
3. If everything didn't go fine, the system reverts the changes and restores the database as it was.
4. If everything went fine, creates a new commit for the addition.

## Remove package

`unboxme [__PROJECT__] remove __PACKAGE__`

Short version: `nb [__PROJECT__] --__PACKAGE__`

1. Uninstalls the package
2. Removes the package from database
3. Removes the code from the system.
4. Commits the changes to git.

## Stage

`unboxme [__PROJECT__] stage [__LOCATION__]`

Short version: `nb [__PROJECT__] -s  [__LOCATION__]`

## Deploy

`unboxme [__PROJECT__] deploy [__LOCATION__]`

Short version: `nb [__PROJECT__] -d [__LOCATION__]`

## Navigate / Switch to a project from anywhere

`unboxme __PROJECT__`

Short version: `nb [__PROJECT__]`

* Terminates any other current running project and initates __PROJECT__.
* Will also set the title of the terminal to read __PROJECT__ in uppercase. 

## Destroy project

`unboxme [__PROJECT__] destroy`

Short version: `nb [__PROJECT__] destroy`

## Upgrade unboxme on your machine

No need, UnboxMe is always up to date!

## Uninstall unboxme from your machine

`unboxme uninstall`

If you f*cked everything up, just delete the ~/boxes/.unboxme folder.

## Extend unboxme with extensions

`unboxme extend __EXTENSION__`

Extensions is also listed here: http://github.com/unboxme/extenstions.
They are mostly used to extend UnboxMe with functionality such as automatic tweets, 
github auto-branching and auto-tagging for every live-deploy.

## Combining multiple commands, examples

### Create a project from sample and stage it.

`unboxme backend-boys drupal-7.x stage`

Short version: `nb backend-boys drupal-7.x -s`

1. Creates new project "backend-boys" from sample "drupal-7.x"
2. Navigates to project
3. Initates project environment
2. Builds and installs as usual with new projects
3. Stages project to for example: fingerstache-wolf.unbox.me

### Re-build, re-install and open in browser.

`unboxme backend-boys build install open`

Short version: `nb backend-boys -bio`

1. Navigates to project "backend-boys"
2. Initates project environment
2. Builds the project
3. Installs the project
4. Opens project in default browser

### Create a project from sample, add packages, build, install and open in browser.

`unboxme frontenders drupal8 open add bootstrap add account-social`

Short version: `nb frontenders drupal8 -o +bootstrap +account-social`

1. Creates new project "frontenders" from sample "drupal8"
2. Adds "bootstrap" package
3. Adds "account-social"
4. Builds and installs as usual with new projects
5. Opens project in default browser


## Manual

`unboxme man`
