
## Hypertag.js
#### Object-Oriented HTML

Hypertag is a runtime for wealthy web applications.  It allows you to serve static files that become limitlessly-flexible interfaces in the user's web browser.


## Hypertag Features

* Templated View objects
* Anonymous Views
* Event-driven View instantiation
* **Infinite recursion** for Views
* Arbitrary attribues and methods on Views
* Attribute inheritance
* Unified view-model architecture
* Deeply-granular init events for Views
* Recursive bubbling of events
* Rich UI events
* Data-driven lists (can be lists of templated Views)
* Drag and drop with definable types
* Elegant **hitches** syntax for dynamic and recursive element resizing
* Global events
* Point-to-point events
* Easy hierarchy navigation
* Simple View removal
* Garbage collection
* Modular XML syntax
* Optional whitespace-delimited syntax
* CSS verbs

At its core, Hypertag is a web app language where templates are *object classes* and views are instances of those classes. Despite its towering list of features Hypertag syntax is shockingly flexible and elegant. The very simplest view is instantiated with just three lines of code.

If you've used Angular, Moustache, or other HTML template engines, some of these features will sound familar.  Hypertag does everything they do and more *and better*.

This may sound like hyperbole but it's simply true.


## Devlopment Advantages

Hypertag lets you write web UIs as self-contained text units. Element design and element logic are a single block of code. These copy/pastable modules allow you to easily port features and widgets between projects.  *Reusability* is a core feature of the language.

Hypertag ends the problem of code speghetification.  Delegation of design work within and between teams becomes efficient.  Dynamic UI items can be shared between authors and slotted into place without requiring every coder to grok everyone else's work.

Normally when you add new features to a web application the complexity grows exponentially.  Hypertag flattens this back to linear growth. Likewise, refactoring a Hypertag project requires a tenth the time.


## Implentation Advantages

Hypertag is fast, efficient, and entirely client-side.  Web applications are meant to be fetched once by the user. All subsequent server interactions are simple AJAX requests for JSON.

With a properly-designed Hypertag application your sever will never have to dynamically compile HTML.  You can throw away CGI, PHP, and other server-side hypertext compilation languages.

Depending on your application requirements, this could cut your infrastructure requirements by an order of magnitude.  *Or more.*
Of course Hypertag can also be integrated with extant web projects.  It takes care not to pollute the DOM or JS namespace, so a Hypertag module can live alongside your existing  code.


## View Model Architecture

In other application languages Views and data models have an independent existence. They may be bound by a set of methods, but they are separate.  In Hypertag view and model are one. The data structure that defines a view element exists as attribute on it.  When you reload a View its data are refreshed, and so are all the data on the views nested inside it.  Removing a view hierarchy and all the data associated with it is as simple as calling its *.remove()* method.  Garbage collection is automatic.


## Events

Hypertag provides a large set of built-in events.  These can be subscribed to via the listen() method and triggered with the set() method.  Listeners can be bound to views, and removed with garbage collection, or they can be global. You are not limited to the built-in events either. *Any* attribute of any JS object can be listened to. There is no limit to the number of listeners.  When bound to views, listens are recursive and bubble appropriately.  You can create complex event chains as you see fit.


## Core Dependencies

* [JQuery|https://jquery.com/]
* [JQuery-templates|https://github.com/BorisMoore/jquery-tmpl]

JQuery is falling out of vogue with web developers.  JQuery Templates was deprecated before the Hypertag project started.  In full awareness of this, these underlying runtimes were still chosen for certain advantages not available in newer libraries.  Several times Hypertag was refactored with other template engine cores to evaluate performance.  Nothing else provides an adequate foundation for Hypertag's fundamental, non-negotiable feature: ***infinite recursion***.


#### Development dependencies

Hypertag provides a rich set of error-reporting and handling to aid the developer. Along with the broswer console and your favorite code editor they provide application authors a solid IDE.

These can be removed for production.

## History

Hypertag was concieved by James Robey and Daniel Swartzendruber in 2010, initially to solve certain issues with a web-based messaging application.  It is the product of over three years of full-time development, and another two of part time developemnt.

99.9999999% of all direct code work was done by James Robey, with Daniel Swartzendruber acting as part-time researcher, sounding board, and documentation writer.  It is the culmination of James's 20 year career as an application language designer.  It incorporates concepts and algorithms he spent his entire life developing.

James passed away in Febuary of 2016, leaving Daniel to curate his work. It was James's intent this library eventually be made open source, after a period of private commercial use.  These plans were cut tragically short.

In tribute to his memory, to preserve his legacy, and honor his wishes, I am forking James's repo and including the uncompiled source.  This is the first time it has been released.  It is under a BSD license with the approval of his heirs.


## Roadmap

1. Maintain both development and production versions as separate directories within the repo
2. Recover and merge the latest version of Hypertag.js, which included updates for mobile
3. Include getting started HTML example.


## The Hypertag Project: HTML "Unleashed"

Find out more at the homepage: [http://hypertag.io|http://hypertag.io]
