PCR V 0.2.0
=========

### "pebble custom reset"

An addition to Eric Meyer's awesome [CSS Reset.](http://meyerweb.com/eric/tools/css/reset/)

PCR uses [SASS](http://sass-lang.com/) to compile a custom reset based on Eric Meyer's reset with a few additions. 

### Dependencies 

PCR requires [SASS](http://sass-lang.com/) if SASS is not already installed there are instillation instructions [here](http://sass-lang.com/tutorial.html)

### Usage

To use PCR follow these simple steps

1. Copy `_PCR.scss` into your projects sass directory. (this can be found in /sass/).
2. Add the line `@import "PCR";` to your main .scss file.
3. PCR is now ready to go. Without specifying any variables PCR will compile Eric Meyer's css reset with no additions.
4. Add variables. To enable the PCR additions you needs to add some variables to your .scss file **above** `@import "PCR";`
