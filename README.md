# packagecheck

There is a movement towards using packages for everything when developing Meteor applications (the [Telescope][1] project is a perfect example of this philosophy). Structuring Meteor applications [in this way][2] has many advantages, however it does pose one annoying issue - it's no longer possible to run `meteor list` to see if there are any updates to packages that you're using.

`PackageCheck` is a command-line that addresses this shortcoming by checking to see if package dependencies used by a Meteor package are themselves up to date.


## Installation

	npm install -g packagecheck

## Usage

    Usage: packagecheck [package-folder-path] ...
           packagecheck --version

With no arguments, `packagecheck` will check the current directory, which can either be a single package or a Meteor 'packages' folder (in  which case all the individual packages will be checked).

Alternatively you may pass in paths to either individual packages and/or 'packages' directories.


[1]: https://github.com/TelescopeJS/Telescope
[2]: https://meteor.hackpad.com/Building-Large-Apps-Tips-d8PQ848nLyE
