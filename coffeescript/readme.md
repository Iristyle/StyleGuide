## Code Style

--

* Use soft-tabs with a 2 space indent
* Maximum 80 characters per line
* Write inline tomdoc for any *public* methods
* [Allman style braces](http://en.wikipedia.org/wiki/Indent_style#Allman_style)
* Style will be enforced with [CoffeeLint](http://www.coffeelint.org/)
and [JsHint](http://www.jshint.com/)
* Use semi-colons ```;``` as line terminators

## Practices

--

* All code should have accompanying tests as documentation
* Major code blocks should have markdown readme in root of repo
* Try to standardize on plugins that will be used rather than selecting things
willy-nilly

## jQuery Guidlines

--

* Prefix jQuery objects with $
* Use jQuery instead of $ in document ready handler

```coffeescript
jQuery ->
  ## your handler here ##
```
* Keep selectors as simple as possible - limit to IDs, tags and classes for
perf reasons (don't use pseudo-selectors like :animated)

```coffeescript
## by id
jQuery '#id'
## by tag
jQuery 'div'
## by class
jQuery '.class'
```
* Cache jQuery objects if used more than once (or chain where appropriate)

```coffeescript
## BAD!
jQuery('#id').css('color:red;')
jQuery('#id').hide()
## GOOD!
jQuery('#id')
	.css('color:red;')
	.hide()
```

## Project Naming Guidelines

--

* Test projects should always end in .Tests as convention to be picked up by
build process

## Frameworks

--

### Testing Tools / Frameworks
* [Mocha](http://visionmedia.github.com/mocha/) - Can run in command line via
node.js or within browser (like QUnit) or via headless like PhantomJS
* [Chai](http://chaijs.com/) - Should / Expect BDD and Assert syntax support
* [Sinon.JS](http://sinonjs.org/) - test stubs, spies and mocks for JavaScript
can fake Ajax requests

### Test Runners - Pick Many
* [Node.js](http://nodejs.org) - Most new JS frameworks can run regular JS code
against node
* [PhantomJS](http://phantomjs.org/) - Full web stack, no browser required
* [Zombie.js](http://zombie.labnotes.org/) - Headless browsing for node
* [Buster.JS](http://busterjs.org/) - Buster is an up and comer, but not sure
its ready for prime-time just yet.  Has the ability to browser automate like
JsTestDriver, qunit static style html page testing and headless phantomJS /
jsdom
* [JsTestDriver](http://code.google.com/p/js-test-driver/) - Can automate actual
browser instances

### Additional Reference

* [Idiomatic Js](https://github.com/rwldrn/idiomatic.js)
* [Common CoffeeScript Idioms](http://arcturo.github.com/library/coffeescript/04_idioms.html)
* [Javascript Style Guides and Beautifiers](http://addyosmani.com/blog/javascript-style-guides-and-beautifiers/)
* [Node](http://nodeguide.com/style.html)
* [Styles in Node Community](http://dailyjs.com/2012/01/12/style/)* [Github styleguide](https://github.com/styleguide)
* [Nerd Kitchen CoffeeScript](http://nerdkitchen.org/blog/coffeescript-style-guide/)
* [PolarMobile CoffeeScript](https://github.com/polarmobile/coffeescript-style-guide)
* [CoffeeScript Idioms](http://arcturo.github.com/library/coffeescript/04_idioms.html)
* [jQuery Core Style Guide](http://docs.jquery.com/JQuery_Core_Style_Guidelines)
* [Google Javascript Style Guide](http://google-styleguide.googlecode.com/svn/trunk/javascriptguide.xml)
* [Annotated Google Style Guide](http://blog.founddrama.net/2010/08/annotated-google-javascript-style-guide/)
* [JavaScript (and jQuery) dev style](https://gist.github.com/1633966)
* [Dojo](http://dojotoolkit.org/community/styleGuide)
* [Aloha Editor](http://aloha-editor.org/guides/style_guide.html)
* [Dart](http://www.dartlang.org/articles/style-guide/)
* [AirBNB Javascript Style Guide](https://github.com/airbnb/javascript)