##This project was designed to provide SVG support for Internet Explorer 6-8. Now that IE natively supports SVG, this project is no longer supported. It is present here for archival purposes only now. The original SVN based repo is at [here](https://code.google.com/p/svgweb/downloads/list). Original docs:

#Overview

SVG Web is a JavaScript library which provides [SVG](http://en.wikipedia.org/wiki/Scalable_Vector_Graphics) support on many browsers, including Internet Explorer, Firefox, and Safari. Using the library plus native SVG support you can instantly target ~95% of the existing installed web base.

Once dropped in you get partial support for SVG 1.1, SVG Animation (SMIL), Fonts, Video and Audio, DOM and style scripting through !JavaScript, and more in a small library. Your SVG content can be embedded directly into normal HTML 5 or through the OBJECT tag. If native SVG support is already present in the browser then that is used, though you can override this and have the SVG Web toolkit handle things instead. No downloads or plugins are necessary other than Flash 10 which is used for the actual rendering, so it's very easy to use and incorporate into an existing web site.

This project is currently in Beta stage development. Many essential SVG features have been implemented but many other features have not been implemented such as filters (except blur, which is implemented) and CSS. Of the remaining features to be developed, some may never be developed, such as advanced filters, unless flash provides a reasonable way to do it.

It should also be noted that while Google has contributed to this project, Google is not providing support for this project.

#One Minute Intro

Quick intro video to SVGWeb:

[![Quick intro video to SVGWeb](http://img.youtube.com/vi/XCk22AaRxiE/0.jpg)](http://www.youtube.com/watch?v=XCk22AaRxiE)

#Demos

  * [Draggable photos demo (scripted with JavaScript + SVG Image tag](http://codinginparadise.org/projects/svgweb/samples/demo.html?name=photos&svg.render.forceflash=false)
  * Bouncing ball demos: [1](http://codinginparadise.org/projects/svgweb/samples/javascript-samples/svg_dynamic.html), [2](http://codinginparadise.org/projects/svgweb/samples/javascript-samples/svg_dynamic_fancy.html)
  * [Draggable videos demo with live video playing (scripted with JavaScript + Video tag](http://codinginparadise.org/projects/svgweb/samples/demo.html?name=videos)
  * [Animated Scimitar using Audio tag and Animation (SMIL) tags](http://codinginparadise.org/projects/svgweb/samples/demo.html?name=scimitar-anim)
  * Simple animation using animation tags (SMIL): [1](http://codinginparadise.org/projects/svgweb/samples/demo.html?name=anim1), [2](http://codinginparadise.org/projects/svgweb/samples/demo.html?name=anim2), [3](http://codinginparadise.org/projects/svgweb/samples/demo.html?name=anim3)
  * [Animating video using tags (SMIL + Video](http://codinginparadise.org/projects/svgweb/samples/demo.html?name=video1)
  * [Animated SVG Open banner with gradients, user-defined fonts (SVG Fonts), and animation (SMIL) tags](http://codinginparadise.org/projects/svgweb/samples/demo.html?name=svgopen)
  * [Defining and using custom fonts (SVG Fonts) demo](http://codinginparadise.org/projects/svgweb/samples/demo.html?name=droid%20font1)
  * Complex static images: [tiger](http://codinginparadise.org/projects/svgweb/samples/demo.html?name=tiger&svg.render.forceflash=false), [sporty car](http://codinginparadise.org/projects/svgweb/samples/demo.html?name=spcar&svg.render.forceflash=false), [techy car](http://codinginparadise.org/projects/svgweb/samples/demo.html?name=techcar&svg.render.forceflash=false techy car)
  * Using viewer to render clip art: [logo](http://codinginparadise.org/projects/svgweb/samples/demo.html?name=android Android), [Cartman](http://codinginparadise.org/projects/svgweb/samples/demo.html?name=cartman), [Mono logo](http://codinginparadise.org/projects/svgweb/samples/demo.html?name=mono)
  * [Falling blocks game](http://codinginparadise.org/projects/svgweb/samples/javascript-samples/blocks_game.html); shows direct embedding SVG into normal non-XHTML HTML 5 and then scripting it with normal JavaScript
  * [Simple 'hello world' showing how to direct embed SVG into normal, non-XHTML HTML 5](http://codinginparadise.org/projects/svgweb/samples/javascript-samples/svg_inline.html?svg.render.forceflash=false)
  * [Simple 'hello world' showing how to use the OBJECT tag (including for IE) to embed SVG](http://codinginparadise.org/projects/svgweb/samples/javascript-samples/svg_object.html?svg.render.forceflash=false)
  * [Simple sample showing how to direct embed multiple SVG into your page](http://codinginparadise.org/projects/svgweb/samples/javascript-samples/svg_inline_multiple.html?svg.render.forceflash=false)
  * [Simple sample showing how to embed multiple SVG OBJECTs into your page and then style them with CSS](http://codinginparadise.org/projects/svgweb/samples/javascript-samples/svg_object_multiple.html?svg.render.forceflash=false)
  * [SVG 1.1 test suite modified to use SVG Web instead](http://codinginparadise.org/projects/svgweb/tests/)

More demos can be seen with the [demo viewer](http://codinginparadise.org/projects/svgweb/samples/demo.html); keep in mind that not all of the demos in the demo viewer work.

#Getting Started

A [Quick Start](http://codinginparadise.org/projects/svgweb/docs/QuickStart.html) guide is available to get going fast. More [in-depth technical documentation](http://svgweb.googlecode.com/svn/trunk/docs/UserManual.html) is also available once you have read the [Quick Start](http://codinginparadise.org/projects/svgweb/docs/QuickStart.html) guide.

#Videos

See a Tech Talk at Google recently on SVG Web and Open Web Advocacy from Brad Neuberg, a member of the Open Web Advocacy team at Google:

[![Quick intro video to SVGWeb](http://img.youtube.com/vi/ctuUrvReOIQ/0.jpg)](http://www.youtube.com/watch?v=ctuUrvReOIQ)

#How to Use

The SVG Web toolkit uses Flash and JavaScript in order to bring static and dynamic SVG to web browsers, including Internet Explorer.

See the User Manual docs/UserManual.html for details on how to use SVG Web.

See the FAQ file docs/FAQ.html for general information.

To see a sample SVG file, view the samples/demo.html file. To see simple examples of using SVG Web in your own projects view the samples in samples/javascript-files/. To run the samples you must have a local web server running; they will not work correctly when run from file:// URLs. If you do not have a local web server the latest build is also running at http://codinginparadise.org/projects/svgweb/

If this is a source distribution, the ActionScript source is in src/org/svgweb/

#What's New

##February 3rd, 2011: New Release!

A new SVG Web release is out, code named Lurker Above.

The Lurker Above is a classic Dungeons and Dragons monster, attaching themselves to dungeon ceilings and dropping down to surprise unwary adventurers:

![Lurker above image](http://codinginparadise.org/images/lurkerabove.jpg)

SVG Web is an open source drop-in JavaScript library that provides SVG support to Internet Explorer 6, 7, and 8 by transparently using Flash.

Some highlights of the Lurker Above release:

  * Internet Explorer 9 is now supported!
  * Lots of bug fixes
  * More SMIL support and fixes
  * Support for SVG Web when used in iframes
  * data-path attribute is now optional and inferred when using SVG Web

Special thanks to Rick Masters for sheparding this release, and to all the bug fixes and help from the SVG Web community!

##August 30th, 2010: New Release

The SVG Web team is proud to announce a new release, code named Owlephant:

![Owlephant image](http://codinginparadise.org/images/owlephant.jpg)

You've heard of Elephants, you've heard of Owls… put them together and you get the fearsome Owlephant. If you encounter one, be sure it will be the last thing you ever, um, encounter. Hoot…. stomp!

With this release we now score 55.45% on the [SVG compatibility charts](http://www.codedread.com/svg-support.php SVG compatibility charts), almost at the same level as IE 9 (58%).

Major aspects of this new release includes overhauls and fixes for gradients, clipping, events, text placement, and more. It also includes a huge step forward in SMIL animation support, including being able to animate path segments and interpolate their values, scripting SMIL with JavaScript, and more.

This release has been built by the community, with major contributions from Bruce Duncan from [VisualMining.com](http://visualmining.com); Ken Stacey from [SVGMaker.com](http://svgmaker.com); and the always awesome (and project co-leader) Rick Masters. Thanks to the many people like Michael Neutze, Bruce Rindahl, and more for their bug testing and evangelism!

See the full ReleaseNotes of what is fixed in this release.

[Download the release now](http://code.google.com/p/svgweb/downloads/list) and [get started](http://codinginparadise.org/projects/svgweb/docs/QuickStart.html)!

Please note that there may be some breaking changes in this release that will affect code that uses older versions of SVG Web; more details [here](http://codinginparadise.org/projects/svgweb/docs/UserManual.html#breaking_changes). Also note that SVG Web does not yet support the native SVG functionality in IE 9 preview releases.

##April 9th, 2010: New Release

I'm proud to announce a new release of SVG Web. Our tradition is to go geek-tastic and name them after classic D&D monsters. This release is named Dracolisk, a crossbreed of a basilisk and a black dragon.

The Dracolisk is a truly fearsome creature, able to turn an enemy into stone with merely the gaze of the basilisk coupled with the acidic breath of a black dragon. Someone get that monster a breath mint.

![Dracolisk image](http://codinginparadise.org/images/dracolisk.jpg)

The fixes and additions in this release:

   * Issue 378: Undefined variable in svg.js source code
   * Issue 435: Regression: test_js1.html and test_js2.html fail
   * Issue 421: Reuse XML ActiveX object on Internet Explorer
   * Issue 431: unsuspendRedrawAll not wired to several methods
   * Issue 428: setAttribute gives error for undefined or null attribute value (Flash renderer)
   * Issue 264: Text with fractional font-size not displayed
   * Issue 405: Support x,y lists on tspan for positioning native font glyphs
   * Issue 440: Text with large font-size displays smaller
   * Issue 447: Text placement changes with different viewboxes
   * Issue 296: appendChild of existing child should move it to the end
   * Issue 462: clipPath outside of def tag renders and blacks out the image
   * Issue 415: Dynamic change of HREF on &lt;use&gt; to different local definition does not work (setAttributeNS())
   * Issue 456: xlink:href attribute on images does not properly change with the Flash renderer
   * Issue 460: Event type is not passed through when mouse events are raised.
   * Issue 465: Stretched images have no smoothing
   * Issue 375: Problem with using svgweb and jquery together
   * Issue 402: Make sure SVG Web and Mootools work together
   * Issue 403: Make sure SVG Web and Prototype.js work together
   * Issue 404: Make sure SVG Web and Ext.js work together
   * Issue 438: Support SVG 'RenderingProperties' CSS Values for Performance Vs. Quality Tradeoffs
   * Issue 437: Slow rendering with mitered corners
   * Issue 452: Parsing complicated long path statements extremely slow
   * Issue 251: data-path configuration via meta tag
   * Issue 332: Formally move to not supporting re-namespacing SVG elements
   * Issue 468: SVG Image regression in test_browser1.html
   * Issue 287: Get large SVG file with lots of PATH nodes where PATH node data has lots of new lines in it faster
   * Issue 466: Semi-legal regex is used in the code.
   * Issue 424: getElementsByTagNameNS(svgns, 'svg')[0] fails in IE7
   * Issue 111: Implement removeEventListener
   * Issue 354: Speed up rxt360's mapping example
   * Issue 409: {{{CurrentScale}}} does not function properly for dynamically created SVG
   * Issue 445: Scripted SVG File Causes Stack Overflow in svgweb
   * Issue 217: replaceChild + setAttribute can lead to display glitches for Flash viewer
   * Issue 181: insertBefore adds object twice which can cause strange display errors

Many thanks from the core SVG Web team (Rick Masters, Brad Neuberg, and James Hight) to the many many contributors to this release, including IBM:

   * Le Roux Bernard
   * Li Yang
   * Jonathan Pasquier
   * Michael Neutze
   * Ken Stacey from svgmaker.com
   * Karl from Zilles.com
   * k5tm from morrisons.us
   * bjtxmql
   * David Stern
   * drjlove
   * Thomas Kelder
   * Gregorio Palama
   * rdworth
   * Evan Adams
   * antihadron
   * alain.couthures
   * Eugene Lazutkin
   * Jeff Schiller
   * Duffy.Ty
   * rxt360
   * don.barthel

[Download the release now](http://code.google.com/p/svgweb/downloads/list) and [get started](http://codinginparadise.org/projects/svgweb/docs/QuickStart.html)!

Please note that there are some breaking changes in this release that will affect code that uses older versions of SVG Web; more details [here](http://codinginparadise.org/projects/svgweb/docs/UserManual.html#breaking_changes).

##November 23rd, 2009: New Release

Just in time for Thanksgiving is another SVG Web release. Our tradition is to name SVG Web releases after monsters from D&D just to increase the geek factor, so in that spirit our release name this time is "Gelatinous Cube":

![Gelatinous Cube image](http://codinginparadise.org/images/gelcube.jpg)

The Gelatinous Cube is a truly horrifying creature:

"A gelatinous cube looks like a transparent ooze of mindless, gelatinous matter in the shape of a cube. It slides through dungeon corridors, absorbing everything in its path, digesting everything organic and secreting non-digestible matter in its wake. Contact with its exterior can result in a paralyzing electric shock, after which the cube will proceed to slowly digest its stunned and helpless prey."

Fun times.

Highlights of this release, thanks to many many people helping with patches, bug testing, and more:

    * Loads of important bugs fixed
    * Performance improvements
    * You can now dynamically create new SVG root tags
    * All the namespace aware functions now implemented: setAttributeNS, getAttributeNS, etc.
    * You can now clone SVG nodes (cloneNode)
    * You can now right-click on the SVG when using Flash to view the dynamic updated SVG source
    * Running getElementsByTagNameNS scoped to a particular node now works, such as myGroup.getElementsByTagNameNS(svgns, 'text')
    * and much much more

The full list of issues fixed:

    * Issue 358: Opera throws exception on patch to currentTranslate
    * Issue 413: Implement node.getElementsByTagNameNS scoped by container node
    * Issue 401: currentTranslate.setXY does translate the svg, but doesn't affect currentTranslate.getX or getY
    * Issue 201: Support cloneNode
    * Issue 385: Implement getAttributeNS
    * Issue 384: Make sure ownerDocument defaults to 'document'
    * Issue 386: Implement hasAttributeNS and hasAttribute
    * Issue 387: Implement removeAttributeNS and removeAttribute
    * Issue 202: Programmatically Creating the SVG node
    * Issue 383: QA on Firefox 3.6 Beta
    * Issue 335: Specific SVG file crashes browser when used with SVG Web
    * Issue 364: onload event does not fire when image url is a security error
    * Issue 362: dynamically applied color should cascade
    * Issue 349: gradients with bounding box cooordinates are positioned wrongly on circles
    * Issue 371: Linear gradients incorrectly start at left of screen rather than each circle
    * Issue 367: Flash blend mode used for groups is a performance problem and can be avoided generally
    * Issue 331: Animations based on events not implemented; problems with transform animations
    * Issue 275: Add View Dynamic Source to context menu
    * Issue 297: Aspect resolution of viewBox not honored on resize of browser
    * Issue 238: SVGImageNode.as should absorb exceptions due to invalid image URL
    * Issue 337: https generates insecure warning with IE6 (FIXED for IE7 and IE8)
    * Issue 388: Cannot Add USE elements dynamically
    * Issue 361: Text label is stealing mouse click
