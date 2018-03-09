# Planning Your Site
## Regions in a Theme
Regions are the **windows** we [talked about before](../ch1/ch1.md#Distributions). They allow content to be seen through them.

Each theme has its own set of regions, designed by the themester (or theme developer). The only **required** region for any theme is the _Content_ region, where the main content goes.

It is not mandatory to use every region available in a theme, but the option is there to use them to peek at content provided by the modules.

Each region has a _name_ and _place_, and site-builders can connect content to a region as they wish.

## Content Entities and Fields
_Content_ is any data that is intended to be displayed to site visitors. In practical terms, this means text, posts, images, files, etc. In Drupal, content is commonly referred to as an _entity_.

Drupal, as a CMS, can manage all sorts of content. Content itself can be pretty vague, making it useful to categorize it into several _types_, almost as equally vague. These types are defined by core or other modules.

Entities _types_ can be further broken down into _sub-types_, and these can have small variations of its display or use, while still maintaining a connection to its parent identity. Sub-types is where the money is.

As an example, the Farmer's Market implementation is going to need to define entities for page content. We can foresee needing three different kinds of pages - a regular one, one that lists a _vendor_ peddling its wares, and one that structures a _recipe_ in a readable, follow-alongable format.

The pages above are all going to be different because they represent information in different ways. They all deal with the same kind of content though (basically title, text, maybe an image), so they'll all be of _type_ **Content item**, defined by the _Node_ module of Drupal's core.

With _sub-types_ we can refine these into the subtypes **Basic Page**, **Vendor Page**, and **Recipe Page**. Each of these entity sub-types are just different kinds of pages that will have access to and layout information in a way particular to them.

We can define what information will be stored for each subtype using _fields_. A sub-type's fields are just the pockets of information available for them to store, and this configuration is shared for each _instance_ of the same sub-type.

Back to our tried and true house analogy:
* **Content** is anything inside the house.
* The **entity type** can be something like _furniture_ (as opposed to wallpaper, or something).
* The **entity sub-type** can further narrow the type of furniture to _sofa_ for instance (other sub-types include dresser, bed, table, etc).
* The **sub-type's fields** are the properties of that sub-type, the information we care to store in that context. For a sofa it might be _comfiness_, _color_, _ruggedness_, _old_person_smell_factor_, _number_of_seats_, etc. All sofas will have this collection of fields about them.

## Modular Content
The seperation of the amorphous blob that is _content_ into entity types is useful as a way of seperating different types of data into their own little classes with identity.

This also makes the content _modular_, which means content can stack on other content and create the composition of a page, pulling information from different places.

This is also the mantra behind _module development_. Modsters (or module developers) need to create their extra functionality as a module that can be easily slotted in and out of a Drupal site.

---

* Previous: [Chapter 1 - Understanding Drupal](../ch1/ch1.md)
* Next: ~~[Chapter 3 - Installation]~~