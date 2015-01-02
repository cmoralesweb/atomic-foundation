Atomic Foundation
=================

Foundation CSS + Atomic Design + SASS Placeholders

#Usage
Inside your bower components installation, you will find a "user-files" folder. Those are files intended to be customized so **you MUST NOT** edit them directly there. Instead, **you MUST copy all "user-files" contents to another directory** (PROJECT_ROOT/SCSS , for example) and edit *that copy*. Modify variables (or add new ones), include or exclude elements commenting them, etc.

Some files import other partials from the bower components directory. You need to adjust that path to your case, doing a search and replace (search for ```@import "ROUTE_TO_BOWER_COMPONENTS/```).

#How to use the placeholders
If you want to use the foundation placeholders, you **MUST** first import their 
regular foundation counterpart. For example, to use grid-placeholders, you must do this:

```
@import "ROUTE_TO_BOWER_COMPONENTS/foundation/scss/foundation/components/block-grid";
@import "ROUTE_TO_BOWER_COMPONENTS/atomic-foundation/foundation-placeholders/block-grid-placeholders";
```

Then, though not mandatory, it's recommended that you turn off classes output:

```
$include-html-block-grid-classes: false;
```

That way, only the classes that you need reach the compiled stylesheet.

#Resources

- Semantic way to use SASS placeholders : http://ianstormtaylor.com/oocss-plus-sass-is-the-best-way-to-css/
- Atomic design with SASS: http://www.smashingmagazine.com/2013/08/02/other-interface-atomic-design-sass/