# Assignment 2

## Introduction 

For this assignment, I kept the same documents that I mentioned for my first submission :

- [THE PRESIDENT IS GONE ZINE][https://archive.org/details/presgone-zine-online/page/n8/mode/1up] by Angélica / H34RTCORE

The two others fanzine come from a collection named Sprout Distro on Internet Archives by the user Various, they are much larger but I didn't find anything interesting and smaller. I may change these two zines if I find something more suitable.

- [DIY Guide to preventing sexual assault][https://archive.org/details/DiyGuideToPreventingSexualAssault/mode/1up] by anonymous, distributed by sproutdistro.

- [ Why Zines Work: A DIY Information Theory ][https://archive.org/details/z_lxxxx/page/n7/mode/2up] by Morgan Stern / Ladyfingerpess

## Assignment 1 DTD Vs Assignment 2 TEI

### What did TEI did better than my DTD

My previous DTD was already inspired by TEI guidelines with the use of a header, followed by a front cover unit, and page divisor unit and a back cover unit. I did not think about bringing the ark reference identifying number into my DTD, even if the Internet Archive create this id for everything stored in their collections. TEI do a better job than me to seperate a lot of authority statement (author, editor, distributor, ressources identifier) but it can be a very repetitive and verbose. I thought of using and external list for <editionStmt> and avoid repetition, but I also thinked that it was to important to be put appart in case documents get separated. It was harder to know where each information bit should be written, for example I chosed to use the attribute ref to encode the link to the github.

In the text encoding, I used Front/Body/Back like my previous work. I chosed to use the div1/div2 ... divisor to encode each pages. I inspired myself directly form the form of encoding inside your exercices. Div2 was used to encode a place where a figure is, 


