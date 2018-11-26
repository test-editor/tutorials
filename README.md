# Tutorials

This repository holds all necessary scripts, compose files etc. to locally start and work through tutorials.

## Tour of Heroes

This tutorial series is using the tour of heroes example application used in angular tutorials [see here](https://angular.io/tutorial).

### Start tutorial

In order to start the first tutorial, clone this repository and change into the root folder of this repository (default is `tutorials`).
The tour of heroes tutorials start scripts are all located in the `heroes` folder. Within that folder issue
* `bash run-hero-create-specification` to start the specification tutorial
* `bash run-hero-create-testcase` to start the test case tutorial
* `bash run-hero-testcase-refactored` to start the tutorial that holds the final solution

## Stop / Restart tutorial

Since the running tutorials consume a bit of memory you can always stop tutorials to free some resources. Stopped tutorials can be restarted very quickly (< 1 min).
Stop the tutorials via `bash stop-tutorial` and restart it with the respective start command (e.g. `bash run-hero-create-testcase`).

## Your changes

Your changes within the tutorial will be available as long as you do not start a different tutorial. Each time you start a different tutorial (via `bash run-hero-...`), your changes will be replaced with
the tutorial. (Re)starting the same tutorial however will keep your changes.

Your changes will be lost too, if you delete the respective docker containers (e.g. via `docker rm ....`).

To keep the changes you made, you can run `bash save-repo`. This will create an archive with the whole Test-Editor-Web project files that will not be overwritten!

## System log

The containers write into a log file (`te.log`) in the root folder of the tutorials, that can be watched (`bash watch-log`) to get a glimpse of the inner workings of these containers.

