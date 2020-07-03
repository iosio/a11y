Notes from JSConf video https://www.youtube.com/watch?v=u-5_x_YnVN0

#### document head updates
libs:
- react-helmet
    - handles changes to document head
    - like updating the document title when the page changes
    
    
 ### Change Announcements
 #### Live Announcer
 make changes to page accessible to screen readers
 
 aria-live attribute
 - area-live="polite"
    - will wait till other announcements are complete
 - aria-atomic="true"
    - will make the announcements over again, anytime the content changes
 
 libs:
 - react-aria-live
 - react-a11y-announcer
 
 
 #### Focus
 be mindful of route changes
 - checkout @reach/router for correct focusing 
 and focus elements that need to be focused 
 
 #### context
 specify contextual info to elements - especially icons
 
 - color
    - be mindful of meaning associated to color
    - be mindful of color blindness
    - use high contrast 
    
#### unit testing
- ARIA attribute values
- page title updates
- Focused elements
- announcers etc
- ... others should be caught in linter 

more libs:
- eslint-plugin-jsx-a11y
    - linter
- react-a11y
    - analyzer
- react-aXe
    - auditor
    
links
- react.rocks/tag/Accessible

other
- chrome dev tools - audits
- react docs on accessibility



 