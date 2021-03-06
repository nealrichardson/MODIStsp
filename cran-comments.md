MODIStsp 1.3.4
================
## Test environments

* ubuntu 18.04 on local install, R 3.4.4
* ubuntu 14.04 on travis-ci (https://travis-ci.org/lbusett/MODIStsp/jobs/383285994#L6)
* win-builder (R-devel, R-release)
* windows 10 on local install, R 3.5

## R CMD check results

There were no ERRORs, WARNINGs or NOTEs

## Note on installation on macos 

Build on macos currently fails (also for MODIStsp 1.3.3.1) with error

"ERROR Package required but not available: ‘gWidgetsRGtk2’"

due to erroring in build of package "RGtk2". 

Note that MODIStsp can be however installed by installing RGtk2 beforehand, following
instructions reported here: 

http://lbusett.github.io/MODIStsp/articles/installation.html#installing-on-mac


MODIStsp 1.3.3.1
================

re-submission of v 1.3.3 patching an issue related to missing import of 
gWidgetsRGtk2, leading to NOTES on Solaris, Fedora and OSX builds (see this 
thread on r-package-devel for details: 
https://stat.ethz.ch/pipermail/r-package-devel/2017q3/001790.html)

There were no ERRORs or WARNING. There was 1 NOTE:

   * checking CRAN incoming feasibility ... NOTE
   Maintainer: 'Lorenzo Busetto <lbusett@gmail.com>'

   Days since last update: 4

due to close resubmission. Sorry for this.

For comments on build environments etc. see the notes below concerning v 1.3.3. 

MODIStsp 1.3.3
==============

## Test environments
* ubuntu 17.10 on local install, R 3.4.1
* ubuntu 16.04 on travis-ci (https://travis-ci.org/lbusett/MODIStsp/builds/263768847)
* win-builder (R-devel)
* windows 10 on local install, R 3.4.1 (As for the previous reelease, 
  R CMD check passes if GTK+ library is properly installed and on Windows PATH,
  otherwise the check causes an endless GTK+ installation loop. This seems a 
  common behaviour for packages relying on RGtk2/gWidgetsRGtk2)
* MacOs on rhub:
  
  Build on Maverick works (https://builder.r-hub.io/status/MODIStsp_1.3.3.tar.gz-3ec4e4680884dc9ca4ebca061af09da3)
  
  Build on El Capitain or Sierra is not possible at the moment, due to the lack
  of updated binaries for RGtk2 (https://builder.r-hub.io/status/MODIStsp_1.3.3.tar.gz-c0e71d5c8f0a42ef85157b346255b4bb)
  A workaround solution using oldrel (Maverick) binaries is provided in MODIStsp README and website


## R CMD check results

There were no ERRORs, WARNINGs or NOTEs


## Downstream dependencies

This package has no downstream dependencies.

--------------------------------------------------------------------------------
MODIStsp 1.3.2
==============

## Test environments
* ubuntu 16.10 on local install, R 3.3.3
* ubuntu 14.04 on travis-ci, R 3.3.3 (https://travis-ci.org/lbusett/MODIStsp/builds/222347443)
* win-builder (R-devel)
* windows 10 on local install, R 3.3.3 (R CMD check passes if GTK+ library is
  properly installed and on Windows PATH, otherwise the check causes an endless
  GTK+ installation loop. This seems a common behaviour for packages relying on 
  gWidgetsRGtk2)
* local OS X install, R 3.3.3

## R CMD check results

There were no ERRORs, WARNINGs 

There was 1 NOTE, related to the fact that this is a first submission.

There was a warning in win_builder about the following (possibly) invalid URL:

https://notehub.org/fctdn

I checked it, and it's working.

## Downstream dependencies

This package has no downstream dependencies.
