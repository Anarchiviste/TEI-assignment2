# Assignment 2

## Introduction 

For this assignment, I kept the same documents that I mentioned for my first submission :
- Here is the link to my previous assignment : https://github.com/Anarchiviste/evalXML.git
- My previous encoding was inspired by TEI, with a header for metadata, a front_cover element, a body element, and back_cover element. A need of mine was to be able to encode the format of very complex and visual chunk of textual and artistic creation. In my DTD, there was metadata that contain the form of the text (colour, materials) and texts blocks themselves (printed text, handwritten text).

- [THE PRESIDENT IS GONE ZINE][https://archive.org/details/presgone-zine-online/page/n8/mode/1up] by Angélica / H34RTCORE

The two others fanzine come from a collection named Sprout Distro on Internet Archives by the user Various, they are much larger but I didn't find anything interesting and smaller. I may change these two zines if I find something more suitable.

- [DIY Guide to preventing sexual assault][https://archive.org/details/DiyGuideToPreventingSexualAssault/mode/1up] by anonymous, distributed by sproutdistro.

- [ Why Zines Work: A DIY Information Theory ][https://archive.org/details/z_lxxxx/page/n7/mode/2up] by Morgan Stern / Ladyfingerpess

- As always, I did not use generative IA for any of my work.

## My DTD vs TEI

My previous DTD was already inspired by TEI guidelines with the use of a header, followed by a front cover unit, and page divisor unit and a back cover unit. I did not think about bringing the ark reference identifying number into my DTD, even if the Internet Archive create this id for everything stored in their collections. TEI do a better job than me to seperate a lot of authority statement (author, editor, distributor, resources identifier) but it can be a very repetitive and verbose. I thought of using and external list for <editionStmt> and avoid repetition, but I think that it was to important to be put appart in case documents get separated. It was harder to know where each information bit should be written, for example I choosed to use the attribute ref to encode the link to the github.

In the text encoding, I used Front/Body/Back like my previous work. I choosed to use the <div1> & <div2> ... divisor to encode each unit in a pages (the definition of a unit is not clear to mysef). I inspired myself directly form the form of encoding inside your exercices. <div2> was used to encode a place where a figure is.  

The figure and figDesc element are not as usefull as I wanted them to be. In my DTD, I had incorporated a element that was describing the place of the figure to help represent where to put it. In TEI I did not found that (maybe I just did not dig enough in the documentation).

TEI is great for persName and authority list incorporation. I did not use an exterior authority list because my documents did not use a lot of persName.

- I used a exterior files to encode the rendition attribute with manuscript/printed id for all my files.

- In Why Zine Work, I did a person list, but not an exterior one because it was used only in this file.

- I used external authority id like Wikidata and Viaf for my person list.

TEI element I used a lot :

  - choice to correct errors when I found one


  - I found it was hard to know where to put every bit of information, especially hyperlink to link an author account to their socials medias. I used attributes like source / ref or target, juggling with what I need and what the TEI guidelines give me.

  - In my DTD I was planning to encode informations about collectives of authors or syndicates, but it was not useful for my documents.

  - In TEI, the availability statement is made to be used my big institution with a clear method off classification. I picked easily available zines, but I do not know how to encode the lack of availabillity (for example, a zine is not curated, in my personnal gallery on my phone)





