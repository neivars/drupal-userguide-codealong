# Understanding Drupal
## Drupal as a Content Management System
* **Featured** - Drupal is wrapped around your actual site, giving you the benefits of on-line editing, uniformity, and the ability to scale the site with extra modules and features.
* **General-purpose** - Other CMS are more specific in their purpose (Wordpress for instance), whereas Drupal wraps around more different kinds of site/app, though with a steeper learning curve.
* **Free** - Self-explanatory.

## Modules
A **module** is a package of code and assets that implement a feature and/or allow extended functionality.

Drupal's codebase was written with modular design, which means a lot of its core features are implemented with modules, exposed through their specific APIs:
* **User module** - Managing user accounts.
* **Node module** - Managing basic content.
* **Field / Field UI modules** - Managing content fields.
* **Menu UI module** - Managing navigation menus.
* **Views / Views UI modules** - Making lists, grids and blocks from existing content.

## Themes
A **theme** is the casing that goes over the _content_, exposing it in a specifically structured and styled way.

## Distributions
A **distribution** is a pre-packaged bundle of _modules_ and _theme(s)_ to serve as either a _fully-featured_ website/app or a _starting point_ for developers.

If a Drupal installation was like a **house**:
* The _modules_ would be the functional rooms inside the house. A kitchen module lets you cook, and a TV-room module lets you have access to depressing news.

* A _theme_ is how you paint the house on the outside and where you put the windows, controlling the way others can see what's inside. They'll only see what's cookin' if a window allows the kitchen module to show its output.

* In this (great) metaphor, the _Drupal framework_ composes the walls, basement, roof and front-door of the house. Without rooms inside it's useless, and without appeal and windows it's impenetrable.

## Types of Data
Data can be categorized into two large groups: **permanent** (though mutable, really) and **temporary**.
### Permanent Data
* **Content** - Data that is meant to be displayed to site visitors. The meat of the app. Can be edited.
* **Configuration** - Data that isn't meant to be completely displayed to site visitors, though it affects certain field names, the title of the page, etc. These smaller bits of information supplement the larger chunks of data that comprises _content_.
### Temporary Data
* **State** - Information about the current state of the _site_ (flags, variables, etc). This data tends to change over time as the site is up.
* **Session** - Information about the current state of the _visitor_ (cookies, login timestamp, etc). This data tends to change **a lot** over time as the visitor interacts with the site. Technically this is a subset of State, since that information is saved server-side (making it part of the site's _State_).

## The Drupal Project
The Drupal project is a _FOSS_ (Free and Open-source Software) project that is at the forefront of developing the Drupal CMS.

The [Drupal Association](https://www.drupal.org/association) is a non-profit organization dedicated to supporting the Drupal project and its community, organizing conventions, fundraisers, promoting Drupal, etc.

## Drupal Licensing
Drupal et al is licensed under the [GNU General Public License (GPL) version 2 or later](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html). This means the code can be downloaded, modified, repackaged, hacked apart, used personally and commercially, amongst other things.

It also means that any contrbution to the Drupal project is also under GNU GPL v^2 if distributed. Derivative works, like _modules_ and _themes_, also fall under the same license if distributed.

There is one exception: all content on _Drupal.org_ is copyrighted by its original contributors and licensed under **Creative Commons Attribution-ShareAlike 2.0**. Some sample code in _Drupal.org_ remains GPL v^2 though.

---

* Next: [Chapter 2 - Planning Your Site](../ch2/ch2.md)