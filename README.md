Atomic Foundation
=================

Foundation CSS + Atomic Design + SASS Placeholders

#Usage
Inside your bower components installation, you will find a "user-files" folder. Those are files intended to be customized so **you MUST NOT** edit them directly there. Instead, **you MUST copy all "user-files" contents to another directory** (PROJECT_ROOT/SCSS , for example) and edit them there. Modify variables (or add new ones), include or exclude elements commenting them, etc.   

#How to use the placeholders
If you want to use the foundation placeholders, you **MUST** first import their 
regular foundation counterpart. For example, to use grid-placeholders, you must do this:

```
@import "bower_components/foundation/scss/foundation/components/grid";
@import "foundation-placeholders/grid-placeholders";
```