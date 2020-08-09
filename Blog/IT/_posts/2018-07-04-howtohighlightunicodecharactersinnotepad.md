---
title:  "How to highlight unicode characters in Notepad++"
permalink: /blog/IT/howtohighlightunicodecharactersinnotepad
---

I have text with unicode characters and I want to highlight those characters in Notepad++
1. Open notepad++ with a blank document.
1. Encoding>Encode in ASCII
1. Paste your text
1. Encoding>Encode in UTF8
This will cause the special characters to be highlighted as symbol codes with their ANSI number. 
Use the [ANSI lookup table](http://ascii-table.com/ansi-codes.php) to see their related Unicode number.

Example text:
A m-dash – 
“smart” quotes