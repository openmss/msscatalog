---
title: How to catalog manuscript contents
layout: page
---

(Rough draft in progress,  posted  ***{{ site.time | date:  '%B %-d, %Y' }}***)



## Background references ##


- Image service with [citable images of manuscripts](http://beta.hpcc.uh.edu/tomcat/mss/photos). 
- Brief identifying information about each of these manuscripts is available from the `.csv` files in this github repository:
<https://github.com/openmss/mss/tree/master/collections/mss>.  The files are organized with a single CITE namespace in each file, and are named by the CITE namespace identifier.  Manuscript identifiers beginning with the string `urn:cite:hmt`, for example, are in the `hmt` namespace, and are documented in <https://github.com/openmss/mss/tree/master/collections/mss/hmt.csv> (manuscripts from the Homer Multitext project).  For this cataloging project, the crucial information for each manuscript is its "page model".  This is a simple ordered list of identifiers for each page in the codex. In the file for manuscripts from the HMT project for example, the codex identified as `urn:cite:hmt:codices.msA` (the Venetus A manuscript) has a codex model identified as `urn:cite:hmt:msA`. Within this codex model, individual pages will be further identified with URNs  like `urn:cite:hmt:msA.12r` to refer to folio 12 recto of the codex.
- Summary information about sources for digital images can be found [here](https://github.com/openmss/img_sources/blob/master/sources.csv). 



## The Process ##

Our goal is to pair an identifier for each text in a given manuscript with an identifier for a range of pges in the codex.  We can express text identifiers with CTS URNs;  we can identify a manuscript page, or range of pages, with a CITE Object URN in the "page model" collection for the manuscript.  Our catalog can therefore be represented by a simple pairing of these two URNs, which is available in a `.csv` at the <https://github.com/openmss/msscatalog> repository, in this file:

<https://github.com/openmss/msscatalog/blob/master/catalog.csv>



In the first entry, the CTS URN for the text is:

    urn:cts:greekLit:tlg0012.tlg0012.msA:
  
This URN refers to the Venetus A version of the *Iliad*, and has no appended passage reference, since we are going to index the occurrence of the entire *Iliad*.

The second value in the entry is for the page range:

    urn:cite:hmt:msA.12r-msA.326v

Your task will be to investigate the manuscripts and visually verify the folio ranges for the works they contain. You will be able to find some information in the online resources from which these manuscripts came, but these are somewhat incomplete, hence our need to catalog them completely and explicitly. 

A URN search tool that will help you generate the necessary cts URNs for the text documents. If you have any questions on URN format, or if any issues come up, you can document them in the [issue tracker](https://github.com/openmss/msscatalog/issues/new) for this repository.
