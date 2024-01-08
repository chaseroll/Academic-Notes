---
tags:
  - Utilities
---
01. callout.css

```css
/* Basic div-like callout as a platform for other styling */

.callout[data-callout="div"] {

position: relative;

margin: 0;

padding: 0.5em 0.5em 0.5em 1em;

background: var(--background-primary);

}

  

.callout[data-callout="div"]::before {

content: '';

position: absolute;

left: 0;

top: 30px;

bottom: 30px;

width: 2px;

background: hsl(var(--accent-h), var(--accent-s), var(--accent-l));

border-radius: 0;

}

.callout[data-callout="div"] > .callout-title {

display: none;

}

.callout[data-callout="div"] p,

.callout[data-callout="div"] li,

.callout[data-callout="div"] blockquote {

color: #808080;

}

/* Ensure LaTeX containers use default text color */

.callout[data-callout="div"] mjx-container {

color: var(--text-normal);

}  

/* Specific callout types, if needed */

.callout[data-callout="bug"],

.callout[data-callout="default"] {

color: #808080;

}
```
  
02. graph-theme.css
```css

.theme-dark .graph-view.color-fill-tag {
color: white;
}

.theme-light .graph-view.color-fill-tag {
color: black;
}

```

03. text-theme.css
```css
/* Basic div-like callout as a platform for other styling */

.callout[data-callout="div"] {

position: relative;

margin: 0;

padding: 0.5em 0.5em 0.5em 1em;

background: var(--background-primary);

}

  

.callout[data-callout="div"]::before {

content: '';

position: absolute;

left: 0;

top: 30px;

bottom: 30px;

width: 2px;

background: hsl(var(--accent-h), var(--accent-s), var(--accent-l));

border-radius: 0;

}

  

.callout[data-callout="div"] > .callout-title {

display: none;

}

  

.callout[data-callout="div"] p,

.callout[data-callout="div"] li,

.callout[data-callout="div"] blockquote {

color: #808080;

}

  

/* Ensure LaTeX containers use default text color */

.callout[data-callout="div"] mjx-container {

color: var(--text-normal);

}

  

/* Specific callout types, if needed */

.callout[data-callout="bug"],

.callout[data-callout="default"] {

color: #808080;

}
```

04. custom-highlight.css
```css

/* Custom highlight class for both edit and preview modes */
.markdown-preview-view .custom-highlight, 
.markdown-source-view .custom-highlight {
    background: hsla(var(--accent-h), var(--accent-s), var(--accent-l), 0.15) !important; /* Accent color with 25% opacity for background */
    color: hsl(var(--accent-h), var(--accent-s), var(--accent-l)) !important; /* Accent color at 100% opacity for text */
}
```

05. theme-modifier.css
```css
.theme-dark.minimal-dark-black {
--ui1: #080808;
} 

.theme-light.minimal-light {
--ui1: #f8f8f8;
}
```

06. responsiveness.css
```css
iframe {

max-width: 100%;

height: auto;

aspect-ratio: 16 / 8; /* Adjust this ratio to match the content */

}

  
  

mjx-container {

font-size: 100%; /* Default font size */

}

@media (max-width: 1200px) { /* When the viewport width is 1200px or less */

mjx-container {

font-size: 100%; /* Scale the font size with the viewport width */

}

}

@media (max-width: 850px) { /* When the viewport width is 800px or less */

mjx-container {

font-size: 75%; /* Minimum font size */

}

}
```
