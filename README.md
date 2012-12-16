# Skeleton framework in SCSS

This is essentially a personal mish-mash between the [Skeleton framework](https://github.com/dhgamache/Skeleton) and [lazerwalker's sassified version](https://github.com/lazerwalker/Skeleton-SASS/).

* All scss files are placed in the stylesheets/scss directory
* Generated stylesheet is in stylesheets/css/style.css


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

Go to the stylesheets directory and run this command:

    sass --watch scss:. --style compressed
