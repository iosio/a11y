make the web accessible to people with disabilities 

also design for mobile, older users

can be beneficial for search engine optimization 

some cant use mouse - revert to keyboard input - then speech

images should have alt text

audio should have transcripts

ATAG (Authoring Tool Accessibility Guidelines)

- support accessible authoring practices;
- generate standard markup;
- support the creation of accessible content;
- provide ways of checking and correcting inaccessible content;
- integrate accessibility support into the overall look and feel of the product;
- promote accessibility in help and documentation; and
- ensure that the tool is accessible to authors with disabilities.


The World Wide Web Consortium (W3C) Web Accessibility Initiative (WAI) 
develops web accessibility standards for the different components:

Authoring Tool Accessibility Guidelines (ATAG) addresses authoring tools

Web Content Accessibility Guidelines (WCAG) Overview addresses web content, 
and is used by developers, authoring tools, and accessibility evaluation tools

User Agent Accessibility Guidelines (UAAG) addresses web browsers and media players, 
including some aspects of assistive technologies


ARIA, the Accessible Rich Internet Applications 
Suite, which defines a way to make web applications more accessible to people with disabilities. 


- content - the information in a web page or web application, including:
    - natural information such as text, images, and sounds
    - code or markup that defines structure, presentation, etc.
- web browsers, media players, and other “user agents”
- assistive technology, in some cases - screen readers, alternative keyboards, switches, scanning software, etc.
- users’ knowledge, experiences, and in some cases, adaptive strategies using the web
- developers - designers, coders, authors, etc., including developers with disabilities and users who contribute content
- authoring tools - software that creates websites
- evaluation tools - web accessibility evaluation tools, HTML validators, CSS validators, etc.



perceivable
    - Text alternatives for non-text content
        - images, icons, buttons, graphics, charts, audio, video
        - labels for forms, controls, input
        - files and formats
        - embedded applications
        - aid in keyboard navigation and voice recognition
    - Captions and other alternatives for multimedia
    - Content can be presented in different ways
    - Content is easier to see and hear
    - meaningful sequence
    -  only one ```<main>``` and ```<footer>```
    - if more than one ```<nav>``` or ```<form>``` use unique id
    - sensory characteristics
        - make sure semantics can be perceived by aria labels
```html
<label for="dogtype">
    Type
</label>
<input aria-describedby="type" aria-labelledby="dogtype"/>
<p id="type">
    The type of dog
</p>
```
    
operable
    - keyboard navigation
    - keyboard focus does not get trapped in content
    - no time limits, user is warned and data is saved if session ends
    - users can easily navigate and find content
        - skip to main content link
    - update title of page 
        
```html
<nav>
    <a href="#skip-to-main">skip</a>
    ...
</nav>
<main id="#skip-to-main">

</main>
```
   
understandable
robust - different assistive technologies 
    - Robust content is compatible with different browsers, assistive technologies, and other user agents. 
    Examples of how this can be achieved include:
        - Ensuring markup can be reliably interpreted, for instance by ensuring it is valid
        - Providing a name, role, and value for non-standard user interface components
    
