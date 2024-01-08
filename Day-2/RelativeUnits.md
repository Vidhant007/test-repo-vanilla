% -> Relative to parent element's value property
em -> Relative to current font-size of the element
rem -> Relative to font size of the root element typically html tag or by default broser defaults

rem :  It allows for consistent sizing relative to the base font size.
ex :
css file :

html {
  font-size: 16px; /* Set the base font size for the root element */
}

body {
  font-size: 1.5rem; /* 1.5 times the root font size (16px), resulting in 24px */
}

h1 {
  font-size: 2rem; /* 2 times the root font size (16px), resulting in 32px */
}

p {
  font-size: 1rem; /* 1 times the root font size (16px), resulting in 16px */
}


em : Relative to font size of closest parent with a specified font size. If no parent with a specified font size exists, relative to browser's  font size is used. 
---> Used for compounding the  size

ex :
css file :

body {
  font-size: 16px; /* Set the base font size for the body */
}

.container {
  font-size: 1.5em; /* 1.5 times the font size of the parent (body), resulting in 24px */
}

p {
  font-size: 1.2em; /* 1.2 times the font size of the parent (container), resulting in 28.8px */
}


NOTE : bot em and rems are not just used for font-size but for all dimensions
ex css :


html {
  font-size: 16px;
}

.container {
  width: 20rem; /* 20 times the root font size (16px), resulting in 320px */
  height: 10rem; /* 10 times the root font size (16px), resulting in 160px */
}

.box {
  width: 2rem; /* 2 times the root font size (16px), resulting in 32px */
  height: 1.5rem; /* 1.5 times the root font size (16px), resulting in 24px */
}
