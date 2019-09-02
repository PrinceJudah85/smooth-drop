Smooth Drop
===========
*NOT MAKING ANY CHANGES TO THIS CODE. ONLY GETTING FAMILIAR WITH GITHUB*

A CSS module for adding *smooth* "cubic-bezier" animation to Bootstrap dropdown menus.

## Install

```bash
npm i smooth-drop
```

## CSS

```css
/*
//
// Smooth Drop
// --------------------------------------------------
*/

.dropdown-menu {
  display: block;
  opacity: 0;
  -webkit-transform-origin: top;
          transform-origin: top;
  -webkit-transform: scale(1, 0);
          transform: scale(1, 0);
  -webkit-transition: opacity 0.1s, -webkit-transform 180ms cubic-bezier(0.3, 0, 0, 1.3);
  transition: opacity 0.1s, -webkit-transform 180ms cubic-bezier(0.3, 0, 0, 1.3);
  transition: opacity 0.1s, transform 180ms cubic-bezier(0.3, 0, 0, 1.3);
  transition: opacity 0.1s, transform 180ms cubic-bezier(0.3, 0, 0, 1.3), -webkit-transform 180ms cubic-bezier(0.3, 0, 0, 1.3);
  -webkit-backface-visibility: hidden;
          backface-visibility: hidden;
}

.dropdown-menu li {
  visibility: hidden;
}

.dropdown-menu.dropdown-menu-center {
  -webkit-transform-origin: top center;
          transform-origin: top center;
  -webkit-transform: scale(0);
          transform: scale(0);
  -webkit-transition: opacity 0.1s, -webkit-transform 180ms cubic-bezier(0.3, 0, 0, 1.3);
  transition: opacity 0.1s, -webkit-transform 180ms cubic-bezier(0.3, 0, 0, 1.3);
  transition: opacity 0.1s, transform 180ms cubic-bezier(0.3, 0, 0, 1.3);
  transition: opacity 0.1s, transform 180ms cubic-bezier(0.3, 0, 0, 1.3), -webkit-transform 180ms cubic-bezier(0.3, 0, 0, 1.3);
}

.open > .dropdown-menu {
  -webkit-transform: scale(1, 1);
          transform: scale(1, 1);
  opacity: 1;
}

.open > .dropdown-menu li {
  visibility: visible;
}

.dropup .dropdown-menu {
  -webkit-transform-origin: bottom;
          transform-origin: bottom;
}

.dropup .dropdown-menu.dropdown-menu-center {
  -webkit-transform-origin: bottom center;
          transform-origin: bottom center;
}
```

## License

The MIT License (MIT)

Copyright (c) 2016 Jason Melgoza

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
