---
layout: page
title: "Indexing scholion markers"
---

For the Upsilon 1.1 or Venetus B manuscripts, scholion markers within the *Iliad* text link passages in the *Iliad* to scholia.  We need to record these after editing the scholia.

## Create an index file

1.  In your repository, please create a directory (folder) named `scholion-markers`
2.  In the `scholion-markers` directory, create a file with a name ending in `.cex`
3.  Add this heading line to the `cex` file:

    `reading#image#scholion#linked text`


## Entries in your index file

Each line represents one entry, with four pieces of information.

1.  The reading of the marker.  Use HMT XML markup as you would in your edition.  For example, if the marker is a Greek numeral 1, you should record `<num>α</num>`
2.  A region of interest on an image illustrating the marker and the Iliadic word it is placed over.
3.  The CTS URN for the scholion this marker links to.
4.  A CTS URN for the *Iliad* line that is linked, including a subreference (beginning `@`) identifying the word that is marked.

## Example

Here is a valid entry:

    <num>Θ</num>#urn:cite2:hmt:vbbifolio.v1:vb_128v_129r@0.5227,0.6307,0.03371,0.03202#urn:cts:greekLit:tlg5026.vb:129r_9#urn:cts:greekLit:tlg0012.tlg001.vb:10.1@παρὰ


Breaking out each part:

1.  `<num>Θ</num>` is the reading (numeric 9)
2.  `urn:cite2:hmt:vbbifolio.v1:vb_128v_129r@0.5227,0.6307,0.03371,0.03202` is the image reference (illustrated below)
3.   `urn:cts:greekLit:tlg5026.vb:129r_9` is the URN for the scholion linked to this passage
4.  `urn:cts:greekLit:tlg0012.tlg001.vb:10.1@παρὰ` is the *Iliad* passage

![](http://www.homermultitext.org/iipsrv?OBJ=IIP,1.0&FIF=/project/homer/pyramidal/deepzoom/hmt/vbbifolio/v1/vb_128v_129r.tif&RGN=0.5227,0.6307,0.03371,0.03202&wID=150&CVT=JPEG)
