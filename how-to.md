---
title: How to...
layout: page
---


Here is our current database of [citable imgages of manuscripts](http://beta.hpcc.uh.edu/tomcat/mss/photos). 

Additional catalog info on the manuscripts may be found [here](https://github.com/openpaleography/mss/tree/master/collections/mss).There is a csv file for library we have taken images from.

Finally, additional information on the source libraries can be found [here](https://github.com/openpaleography/img_sources/blob/master/sources.md). 

## The Process ##

Our first step will be to catalog the folio ranges of different text documents contained within a manuscript. To start we will be focusing on manuscripts we know contain Homeric material (see the list of eight manuscripts above). Later we will move on to additional manuscripts in our database. 

We'll be working in the file called 'catalog.csv.' You will see that it is a two-column, comma-separated-value file. The first value is for the Text URN. This an URN value that will indicate the work you find in the manuscript. Be sure to include the reference to the manuscript in your URNs. The first entry in the file is an example template for you to follow. 

    urn:cts:greekLit:tlg0012.tlg0012.msA:
  
This URN refers to the Venetus A version of the *Iliad*

The second value in the table is for the folio range.

Your task will be to investigate the manuscripts and visually verify the folio ranges for the works they contain. You will be able to find some information in the online resources from which these manuscripts came, but these are somewhat incomplete, hence our need to catalog them completely and explicitly. 

A URN search tool that will help you generate the necessary cts URNs for the text documents. If you have any questions on URN format, or if any issues come up, you can document them in the [issue tracker](https://github.com/openpaleography/msscatalog/issues/new) for this repository.
