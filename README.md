PCR V 0.2.0
=========

### "pebble custom reset"

An addition to Eric Meyer's awesome [CSS Reset.](http://meyerweb.com/eric/tools/css/reset/)

PCR uses [SASS](http://sass-lang.com/) to compile a custom reset based on Eric Meyer's reset with a few additions. 

### Dependencies 

PCR requires [SASS](http://sass-lang.com/) if SASS is not already installed there are instillation instructions [here](http://sass-lang.com/tutorial.html)

### Demo

To get the demo working locally.

1. Clone the repro. `$ git clone git@github.com:pebblecode/PCR.git`
2. Run `$ compass watch` to tell compass to auto compile your css as you make changes.
3. Edit variables at the top of `/sass/style.scss` (See bellow for a list of variables.)
4. Open `index.html`. Refresh to see changes to your reset as they are complied. 

### Standard usage

To use PCR in your own project.

1. Copy `_PCR.scss` into your projects sass directory.
2. Add the line `@import "PCR";` to your main .scss file.
3. PCR is now ready to go. Without specifying any variables PCR will compile Eric Meyer's css reset with no additions.
4. Add variables. To enable the PCR additions you needs to add some variables to your .scss file **above** `@import "PCR";`

### Variables

The following variables can be added to your .scss file **above** `@import "PCR";` to give your reset additional rules. 

#### `$remove-list-styles` 
Set to 'true' to add the following code to your reset.

```css
/* 'true' */
ul, ol {
	list-style: none;
}
```

#### `$link-underline` 
Set to 'none' or 'hover' to add the following code to your reset.

```css
/* 'none' */
a:link{
  text-decoration: none;
}

/* 'hover' */
a:link{
  text-decoration: none;
}
a:hover{
  text-decoration: underline;
}
```

#### `$ins-color` 
Set a color to add the following code to your reset.

```css
/* 'yellow' */
ins{
  background-color: yellow;
}
```

#### `$focus-outline` 
Set a outline property to add the following code to your reset.

```css
/* '1px dotted grey' */
:focus {
  outline: 1px dotted grey;
}
```

#### `$abbr-dfn-styles` 
Set to 'true' to add the following code to your reset.

```css
/* 'true' */
abbr[title], dfn[title] {
  border-bottom: 1px dotted;
  cursor: help;
}
```

#### `$hr-styles` 
Set to 'true' to add the following code to your reset.

```css
/* 'true' */
hr {
display: block;
height: 1px;
border: 0;
border-top: 1px solid #cccccc;
margin: 1em 0;
padding: 0;
}
```

### Credits

Big thanks to [Eric Meyer](http://meyerweb.com/) And [html5doctor.com/](http://html5doctor.com/) 