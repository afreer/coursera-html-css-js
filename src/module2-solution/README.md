
### Project Skeleton

No CSS/javascript frameworks are allowed for this assignment,
e.g. Bootstrap and jQuery are not included.  The project skeleton
is inspired by these frameworks, however.

Overview:

 # Created folders: css, fonts, js, to match Twitter Bootstrap template.
 # Created css and js override files, styles.css and script.js,
    inspired by the course examples.
 # README.md: A little metadata/notes.
 # index.html: The main page.

Files:

    index.html
    README.md
    
    css/
        styles.css
    
    fonts/
    
    js/
        script.js
    
### CSS responsive layout equal column height issue

With the float based layout, adjacent sections with a different amount
of text would end up with different heights.  This looked weird.

I tried a number of things, but ultimately using the relatively new
CSS flexbox styling did the trick fairly nicely.

I abstracted this into two different CSS styling files:
 
 # css/styles-reponsive-float.css
 # css/styles-reponsive-flex.css

You can experiment with the float vs. flex difference by uncommenting/commenting 
the appropriate inclusion lines in index.html.

caniuse.com revealed that "flexbox" support is very good, with 
the possible exception of Internet Explorer. I tested IE11 on an old
Windows 7 box and it still looked good, at least for this small assignment.

These resources were very helpful for understanding flexboxes:
 
 # https://css-tricks.com/snippets/css/a-guide-to-flexbox/
 # There were others, but I think this one was the one that did the trick.

