---
title: Indexing Iliad lines
layout: page
---


Every passage of text we edit is indexed to a physical page, and a documentary image.  When you validate, verify and push to github your paleographic observations, your next assignment is to index *Iliad* lines on your page.

This information about a *documented scholarly edition* goes in the `dse` directory of your repository.  Your files in this directory can have any name ending in `.cex`.  The first line of each file should have the header  line `passage#imageroi#surface`.  Subsequent lines are composed of three URNs separarted by a `#` character:


1.  The CTS URN for the line of the *Iliad*
2.  A CITE2 URN you copied from the image citation tool identifying the region on an image where the line is illustrated
3.  A CITE2 URN identifying the page
