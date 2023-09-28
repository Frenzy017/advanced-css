# advanced-css
Creating advanced css / sass layouts with animations

Three pillars to write good html and css

**Responsive design**

* Fluid layouts
* Media queries
* Responsive images
* Desktop-first vs mobile-first

**Maintainable and scalable code**

* Clean
* Easy-to-understand
* Growth
* Reusable
* How to organize files
* How to name classes
* How to structure HTML

**Web performance**

* Less HTTP requests
* Less code
* Compress code
* Use a CSS preprocessor
* Less images
* Compress mages

**What happens to CSS when we load up a webpage?**

*Loads HTML > Parse HTML > Load CSS > Parse CSS > Create 
DOM / CSS Object model > Renders the tree > Website rendering the visual formatting model > Final rendered Site*

**The Cascade (The "C" in CSS)**
 *- Process of combining different stylesheets and resolving conflicts
between different CSS rules and declarations, when more than one 
rule applies to a certain element.*

**How CSS is parsed & specificity**

*Importance > Specificity > Source Order*

// Importance
1. User :important declarations
2. Author :important declarations
3. Author declarations
4. User declarations
5. Default browser declarations


// Specificity
1. Inline styles
2. IDs
3. Classes, pseudo-classes, attribute
4. Elements, pseudo-elements


// Source order
// Same specificity?
*The last declaration in the code will override all other
declarations and will be applied*

* Css declarations marked with !important have the highest priority
* But, only use !important as a last resource. It's better to use correct 
specificities - more maintainable code!
* inline styles will always have priority over styles in external stylesheets
* A selector that contains 1 ID is more specific than one with 100 classes
* A selector that contains 1 class is more specific than one with 1000 elements
* The universal selector has no specificity value(0,0,0,0)
* Rely more on specificity than  on the order of selectors


**How units are converted from relative to absolute (PX)**

* %(fonts) - x% * parent's computed font-size
* %(lengths) - x% * parent's computed width
* em(font) - x * parent computed font size
* em(lengt hs) - x * current element computed font-size
* rem - x * root computed font-size
* vh - x * 1% of viewport height
* vw - x * 1% of viewport width


**Inheritance: what you need to know**

* Inheritance passes the values for some specific properties
from parents to children - more maintainable code.
* Properties related to text are inherited: font-family, font-size, color etc.
* The computed value of a property is what gets inherited, not the declared value
* Inheritance of a property only works if no one declares a value for that property
* The inherit keyword forces inheritance on a certain property