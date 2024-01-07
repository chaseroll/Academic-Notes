---
tags:
  - Utilities
---
01. callout.css

```scss

/* basic div-like callout as a platform for other styling */

.callout[data-callout="div"] {

position: relative; /* Needed for the absolute positioning of the pseudo-element */

margin: 0;

padding: 0.5em 0.5em 0.5em 1em; /* Adjust padding as necessary */

background: var(--background-primary); /* Adapts to light or dark theme background */

}

  

.callout[data-callout="div"]::before {

content: '';

position: absolute;

left: 0;

top: 30px; /* Fixed distance from the top */

bottom: 10px; /* Fixed distance from the bottom */

width: 2px; /* Width of the sidebar */

background: hsl(var(--accent-h), var(--accent-s), var(--accent-l)); /* Uses accent color */

border-radius: 0; /* Ensures the sidebar has no rounded corners */

}

  

.callout[data-callout="div"] > .callout-title {

display: none; /* Hides the callout title */

}

  

.callout[data-callout="div"] > .callout-content {

margin-left: 10px; /* Space after the sidebar */

}
```
  




02. graph-theme.css
    ```scss
     
    .theme-dark .graph-view.color-fill-tag {
    color: white;
	}
	
	.theme-light .graph-view.color-fill-tag {
	color: black;
	}
	