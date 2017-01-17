# MOLDA - *Responsive Grid System*

Just one more classic grid system. 
I was trying to learn more about grid systems so, i created one.
In a few words, MOLDA is a very simple and highly customizable grid.
[Project page](https://github.com/filipedaniel/MOLDA-Responsive-Grid-System)

## Download
 - Download: [zip](https://github.com/filipedaniel/MOLDA-Responsive-Grid-System/archive/master.zip)

## Quick-Start
``` html
<link rel="stylesheet" href=".../molda.css">
```
MOLDA is based in others big grid systems projects like [*Bootstrap*](http://getbootstrap.com/) and [*Foundation*](http://foundation.zurb.com/) so, the way to use is very similar to them.

#### Exemple
```html
<div class="container">
  <div class="row">
    <div class="column xs-12 sm-6 md-4 lg-3"> ... </div>
    <div class="column xs-12 sm-6 md-4 lg-3"> ... </div>
    <div class="column xs-12 sm-6 md-4 lg-3"> ... </div>
    <div class="column xs-12 sm-6 md-12 lg-3"> ... </div>
  </div>
  <div class="row">
    <div class="column xs-12 sm-offset-3 sm-6"> ... </div>
  </div>
</div>
```
## Default vs Custom

There is many ways to customize MOLDA but all of variables have default values.
To customize just change the *".scss"* file *(molda.scss)* and compile for create new *".css"* file.
List of custom values:

```scss
// If you want to use a container to delimiter your content
$use-container: true !default;

// Names of grid system main classes
$container-name:  "container" !default;
$row-name:        "row" !default;
$column-name:     "column" !default;

// Column numbers
$grid-columns: 12 !default;

// Names of the prefix breakpoints class (ex: xs-12, sm-10, ...)
$xs-name: 'xs' !default;
$sm-name: 'sm' !default;
$md-name: 'md' !default;
$lg-name: 'lg' !default;
$xl-name: 'xl' !default;

// Gutter width
$gutter: 20px !default;

// Width breakpoints
$breakpoint-screen-sm: 576px !default;
$breakpoint-screen-md: 768px !default;
$breakpoint-screen-lg: 992px !default;
$breakpoint-screen-xl: 1200px !default;

// Container max width for the different breakpoints
$container-xs-width: 100% !default;
$container-sm-width: 540px !default;
$container-md-width: 720px !default;
$container-lg-width: 960px !default;
$container-xl-width: 1140px !default;

// compile utilities
$compile-utilities: true !default;
```
##  Compile
Exist a precompiled file in *src* folder. If change any of the variables and want a new compile file:

 - Command Line [SASS Docs](http://sass-lang.com/install)
```
sass -Ct expanded molda.scss molda.css --sourcemap=none
sass -Ct compressed molda.scss molda.min.css --sourcemap=none
```
 - Online:  [Sassmeister](http://www.sassmeister.com/)

 - Software (ex:.)
     - Koala [(Open Source)](http://koala-app.com/)
     - Scout-App [(Open Source)](https://mhs.github.io/scout-app/)
