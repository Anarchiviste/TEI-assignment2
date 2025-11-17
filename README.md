# Introduction 

For this assignment, I kept the same documents as those mentioned in my first submission:

Here is the link to my previous assignment: https://github.com/Anarchiviste/evalXML.git

My previous encoding was inspired by TEI, with a header for metadata, a front_cover element, a body element, and a back_cover element. I needed to be able to encode the format of a very complex and visual piece of textual and artistic creation. In my DTD, there was metadata that contained the form of the text (color, materials) and the text blocks themselves (printed text, handwritten text).

[THE PRESIDENT IS GONE ZINE][https://archive.org/details/presgone-zine-online/page/n8/mode/1up] by Angélica / H34RTCORE

The other two fanzines come from a collection called Sprout Distro on Internet Archives by user Various. They are much larger, but I couldn't find anything interesting that was smaller. I may change these two zines if I find something more appropriate.

[DIY Guide to preventing sexual assault][https://archive.org/details/DiyGuideToPreventingSexualAssault/mode/1up] by anonymous, distributed by sproutdistro.

[ Why Zines Work: A DIY Information Theory ][https://archive.org/details/z_lxxxx/page/n7/mode/2up] by Morgan Stern / Ladyfingerpess

# AI Statement

As always, I have not used any generative AI in my work.

# Reflections on DTD and TEI

My previous DTD was already inspired by TEI guidelines, using a header, followed by a front cover unit, a page separator unit, and a back cover unit. I hadn't thought to include the ARK reference ID in my DTD, even though the Internet Archive assigns this identifier to all documents in its collections. TEI handles the separation of numerous authority statements (author, publisher, distributor, resource ID) better than I do, but it can be very repetitive and verbose. I considered using an external list for `<editionStmt>` to avoid repetition, but I felt it was too important to separate it in case the documents were separated. It was more difficult to know where to place each piece of information; for example, I chose to use the `ref` attribute to encode the link to GitHub.

For text encoding, I used the Front/Body/Back structure, as in my previous work. I chose to use the divider `<div1> & <div2> ...` to encode each unit on a page (the definition of a unit isn't clear to me). I was directly inspired by the encoding method in your exercises. `<div2>` was used to encode the location of a figure.

The `figure` and `figDesc` elements aren't as useful as I'd hoped. In my DTD, I had included an element describing the figure's location to facilitate its placement. I couldn't find this element in TEI (perhaps I didn't explore the documentation thoroughly enough).

TEI is ideal for integrating names of people and authority lists. I didn't use an external authority list because my documents contain few names of people.

- I used an external file to encode the `rendition` attribute with the handwritten/printed identifier of all my files.

- In "Why Zine Work," I created a people list, but not an external list because it was only used within that file.

- I used external authority identifiers like Wikidata and Viaf for my people list. I chose to correct errors as I went along. I found it difficult to know where to place each piece of information, especially hyperlinks connecting an author's account to their social media profiles. I used attributes like source/ref. or target, balancing my needs with the TEI guidelines. In my DTD, I planned to encode information about authors' collectives or unions, but this wasn't relevant to my documents. In TEI, the availability statement is designed for use by a large institution, with a clear classification method. I have selected the easily accessible fanzines, but I don't know how to encode their unavailability (for example, an unarchived fanzine, in my personal gallery on my phone).



