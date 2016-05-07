# XML-TEI Bible Documentation

This file gives some general information of how this project is beeing built.

# Overview

The main file of this project is the TEIBible.xml file, which is in the root of the folder. This projects encodes the books of the Bible one by one not in any previsable order. That explain the fact that only some of the books are (and will be) inside the TEIBible.xml. The other most important file is the ontology.xsl; there you will find the basic information about the people, groups, places, times and books that are encoded in the TEIBible.

All the other files and folders are documentation, extra files or work-in-process files.

## Licence

My work in this project and its markup are published under Creative Commons Licence BY Attribution 4.0 International. The data is available over GitHub and is published as it is. Please, take in consideration that this project lacks of any kind of financial or institutional support, for good and bad.

# Original Idea

I, José Calvo Tello, started this project in 2015 out of pure interest in his free time. I didn't find any version of the Bible in XML-TEI in which information below the verse level was encoded, like references to people and places, or who was talking and to whom. My interest on the Bible awaked the idea of encode such information, which meant another kind of reading and would allow the use of new computational techniques to get more information about the text.

Although this project is not part of my research work, neither I am preparing the data to answer any hypothesis, while working I am using my background as scholar with experience in different areas of philology, NLP and Digital Humanities.

# Text


## Original Text

The original text comes from a Reina Valera translation into Spanish. I didn't take any of the most modern in order to avoid copy right problems.

## Language

The text is in Spanish because is my mother tongue. The project doesn't forsee to export the structure of the markup to other languages, but I could help to develope a strategy of doing it.

## Markup

The text is encoded in XML-TEI and controlled with a scheme, also published in the project. The root element of the TEIBible.xml  is a teiCorpus, which has very basic metadata. Every book is then encoded as a TEI element, with some basic Metadata.

### Chapters, Pericopes and Verses

The books of the Bible are identified using the ids from here: http://www.umiacs.umd.edu/~resnik/parallel/bible/bookcodes.all

In each book, the chapters are encoded as divs, keeping the number of the chapter both in a @n attribute and in the id. The verses follow the same system but are encoded as ab elements (I decided to use it because neither the definition of the p element nor l element fit the concept of the biblical verse).

Between chapters and verses exists a medium level of division, which typically has a title. I call it pericopes (although the pericopes are often used only to this level of division in the Gospels). 
	

### Name entities

### Direct Speech

### 

# Structure of the Markup

The project has started encoding:
* Chapter, pericopes and verses
* References to peoples, places, times, groups and books, using ids
* Direct speech, including who is communicating, to whom and how (written, oral, prayer...)


# Ontology


# Previous Work and Inspiration

# Aditional files


This project also includes some other files:
* Scheme to control the XML-TEI
* CSS to visualize the text in Browser and correct it
* Some files of documentation
* XSLT and Python scripts to extract some interesting information
* The resulting data and visualizations
* CSV file (ontology.csv) to control the ids used


# Thanks to

# Future Work

## Colaboration
If some would have interested to export the structure of the markup to other languages (alive or dead) with some kind of machine learning method, I could help to develope the idea and 



