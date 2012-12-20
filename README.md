# Skeleton framework in SCSS

This is essentially a personal mish-mash between the [Skeleton framework](https://github.com/dhgamache/Skeleton) and [lazerwalker's sassified version](https://github.com/lazerwalker/Skeleton-SASS/).

* All scss files are placed in the sass directory
* Generated stylesheet is stylesheets/screen.css
* Meddle all you want with the base.scss file for your customizations


## Installation

This project now uses [compass](http://compass-style.org/). Reuse is the new small :S

### [compass installation](http://compass-style.org/install/)

    gem install compass
    cd <myproject>
    compass create


## Usage

Unlike the original Skeleton, the sassified version is made to apply to your existing styles e.g.

    .container{ @include container; }

    #header {
      @include columns(16);
    }
    #col1, #col2, #col3 {
     @include columns(5.33);
    }


## Useful commands

### Compile and compress the scss files:

Just go to your project folder and execute below commands:

    # To compile on demand:
    compass compile [path/to/project]
    compass compile [path/to/project] -s nested/expanded/compact/compressed

    #To monitor your project for changes and automatically recompile:
    compass watch [path/to/project]


### Compile and compress the scss files using just sass:

I would just use compass, but if that's not your thing use this command:

    sass --watch sass:../stylesheets/ --style compressed


