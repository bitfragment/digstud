![125%](https://cdn1.iconfinder.com/data/icons/Filecons_light/498/txt.png)

^
* Concept of file →
* Text file: can be "ordinary" text, or (executable) program text
* "Ordinary" text = document

----

![fit](http://upload.wikimedia.org/wikipedia/commons/2/29/Linux_command-line._Bash._GNOME_Terminal._screenshot.png)

^
* Explain: CLI before GUI
* [Show them using my terminal]
* [Show them 2 online editors in course notes]
* The content of this display we call "plain text"
* ?(Plain is contrast with what)
* Fancy: "styled" or "rich" text

----

![175%](http://www.onlineimageeditor.info/images/rich_text.jpg)

^
* ?(Difference between these two kinds of text) [flip back and forth]
* Variable font
* Variable font size
* Variable color
* [Demo with terminal vs. TextEdit- plain convert to rich and manipulate]

----

![fit](http://upload.wikimedia.org/wikipedia/commons/e/e0/ASCII_Code_Chart-Quick_ref_card.png)

^
* USASCII has no formatting codes: font size, italics, underlining, etc.

----

![fit](http://farmdev.com/talks/unicode/images/unichart-100.jpg)

^
* Note does Unicode, even though it contains all writing systems

---

Plain text → formatted with markup → Styled or "rich" text

^
* Formatting is accomplished through additional encoding
* We call that MARKUP

----

![fit](http://www.terums.com/images/pictograms/what%20you%20see%20is%20what%20you%20get.gif)

^
* Text that you see on the screen is what you see if you print it out

----

![fit](http://www.windowsshareware.com/common/img/10042.jpg)

^
* Microsoft Word and other word processors

----

![fit](http://parveenarora.in/sites/default/files/vim.png)

^
* Text editors date from the pre-GUI era, 1970s
* Still in use today, especially by programmers
* [Demo in my terminal using nano]
* [Open Ymacs in browser]
* [Open jsvi in browser]

----

![150%](http://www.trs-80.org/wp-content/uploads/pencil1.png)

^
* Word processors date from the same era, 1970s
* Advertisement [describe: image, price, storage format]

----

![fit](http://upload.wikimedia.org/wikipedia/commons/d/dc/Office_Products_output_samples_1980-81.png)

^
* Goal was to produce text for typesetting of printed material using a printer, rather than programming

----

![200%](http://www.trs-80.org/wp-content/uploads/pencil4.png)

^
* First for a portable computer: Electric Pencil

----

![fit](http://www.vintage-computer.com/images/kaypro10keyboard.jpg)

^
* WordStar, 1980s
* On portable computers like the Kaypro

----

![fit](http://content.answcdn.com/main/content/img/CDE/_WDSTAR.GIF)

----

![fit](http://ozzy.impakt.net/screenshot-wordstar.JPG)

----

     ^BSAMPLE TEXT^B
     
     ^SWordStar^S is a CP/M compatible, screen-oriented processing system with integrated printing capabilities...
     
^
* ?(Anything unusual here?)

----

![fit](http://upload.wikimedia.org/wikipedia/commons/f/f3/Wordperfect-5.1-dos.png)

^
* WordPerfect, 1980s, for DOS

---

![fit](http://upload.wikimedia.org/wikipedia/en/e/e6/Corel_WordPerfect_X3_Reveal_Codes_screenshot.png)

^
* Explain GUI: Mac, Windows, 1980s
* WordPerfect in 1990s

----

![fit](http://images.amazon.com/images/G/01/software/detail-page/B0017I8NQM-3.jpg)

^
* Bottom panel of display: another version of the text in above panel
* Includes formatting markup
* Text added to the plaintext as formatting instructions
* Enabling the WYSIWYG representation in top panel

----

## *Markup*: additional text added to plain text to enable **WYSIWYG** styled or "rich" text

^
* ?(What's the styled text here?)
* [Show them using Deckset's 'edit in' and a new slide → Byword]
* [This is a markup format we'll talk about later]
 
----

## Markup

* Types
* History
* The situation today: the web development “stack”

^
* We’ve been talking about the concept of a document
* A file whose content is text
* Markup formats
* Next 2 sessions: review 3 types, their history
* Much faster than in a web dev course
* Brief non-technical summary of where web dev is today

----

## Three types of markup

1. Processing markup
1. Semantic markup
1. Presentation markup

----

## Processing markup

Producing printed or printable documents

----

## Semantic markup

Describing the structure of documents

----

## Presentation markup

Presenting documents on a screen

----

![fit](http://www.designersinsights.com/wp-content/uploads/2012/03/Big-Type-Capitals.png)

^
* History of processing markup: typesetting
* Taking a handwritten ms. or a typewriter typescript…
* …setting it in type for newspaper/magazine/book publication
* Different sizes, weights, alignments of type on a page
* For different functions

----

![125%](http://www.technical-expressions.com/layout/markup/images/Typesetting-markup-eg50.gif)

^
* Handwritten typesetting markup by copy editor
* Typescript; handwritten instructions [read them]

----

![fit](http://www.marksimonson.com/assets/content/notebook/markup001.jpg)

^
* Handwritten instructions for formatting of typewritten address labels
* [read top to bottom] Alignment; font; instructions at bottom

----

![fit](http://www.j-giampietro.com/blog/wp-content/uploads/2010/02/gblog_manuscript_markup.jpg)

^
* Magazine advertisement
* "Three Basic Truths about Travel"
* Typescript with handwritten instructions: layout, font, etc.
* [read "Attn: Lenny" at bottom]

----

## `TYPSET` and `RUNOFF` (1960s) → 
## `runoff` (1970s) → 
## `roff` (1970s) →
## `nroff` (1970s) → 
## `troff` (1970s)

^
* Printing to line printers and typesetters
* *Electronic* forms of typesetting markup: added characters
* `runoff` = "I'll just run off a copy" (office photocopy lingo)
* [read] runoff shortened to roff, "new roff," "typeset roff"

----

## TYPSET/RUNOFF Markup

When you're ready to order,
call us at our toll free number:
.SK
.CENTER
1-800-264-4656
.SK
Your order will be processed
within two working days and shipped

^
* Formatting codes were inserted into text with instructions for printer/typesetter
* Began with dots, since no normal English words began with dots

----

## TYPSET/RUNOFF output

   When you're ready to order, call us at our toll free number:

                      1-800-264-4656

   Your order will be processed within two working days and shipped

^
* [Toggle back and forth]
* ?(What's different)
* ?(Infer function of formatting codes?)

----

## `troff` source of Unix Seventh Edition Manual (Bell Labs)

^
* [Open troff source and PDF]
* [Show them]

----

![inline,left](http://www.randform.org/blog/wp-content/2006/07/latexplusmetafont.jpg)![inline,right](http://upload.wikimedia.org/wikipedia/commons/9/9c/Latex_example.png)

^
* TeX (1978) and LaTeX (1984) + Metafont typesetting software

----

![inline,left,100%](https://earthsci.stanford.edu/computing/unix/formatting/latexexample8.jpg)
![inline,right,90%](http://i.stack.imgur.com/VweGa.png)

^
* Designed especially for typesetting mathematical equations

----

![fit](https://nclab.com/wp-content/uploads/2013/01/034.png)

^
* LaTeX markup looks like this
* Formatting commands begin with a backward slash and curly braces and square brackets specify values
* ?(Can you guess what this will produce if you compile it)

----

![175%](http://lh4.ggpht.com/_S0f-AWxKVdM/S-U89iSE8wI/AAAAAAAAMSU/d9XHuvFqkuY/latex-input%5B3%5D.png?imgmax=800)

----

![125%](http://upload.wikimedia.org/wikipedia/commons/9/9c/Latex_example.png)

----

## writelatex.com

^
* [open, enlarge font]
* Plain text with markup on left
* Formatted PDF document on right
* [Change title to "My Puppy Is Cute"]
* [Delete below introduction to \end{document}]
* [Explain section headings]

----

1. Processing markup
1. Semantic markup
1. Presentation markup

^
* LaTeX = complex text *processing* markup, for complex typeset PDFs
* So far, we've only discussed that category
* WWW, early 1990s, needed simpler for displaying text in browser
* HTML = markup format to display Web pages
* History → all three types of markup

----

## GML (1960s-1970s) → 
## SGML (1980) → 
## HTML (1990s)

^
* Genealogy: each incorporated features of the previous
* Generalized Markup Language: IBM's internal document formatting markup 
* Standard Generalized Markup Language: standardized semantic (descriptive) markup for cataloging and sharing documents
* HTML: presentation markup for publishing Web pages

----

## GML (Generalized Markup Language)

	  :h1.Chapter 1:  Introduction
	  :p.GML supported hierarchical containers, such as
	  :ol
	  :li.Ordered lists (like this one),
	  :li.Unordered lists, and
	  :li.Definition lists
	  :eol.
	  as well as simple structures.
	  :p.Markup minimization (later generalized and formalized in SGML),
	  allowed the end-tags to be omitted for the "h1" and "p" elements.

^ 
* Like RUNOFF and troff examples we saw, commands beginning with punct
* Describe structural elements of a document [describe]

----

## SGML (Standard GML)

	  <h1>Chapter 1: Introduction</h1>
	  <p>GML supported hierarchical containers, such as
	  <ol>
	  <li>Ordered lists (like this one),
	  <li>Unordered lists, and
	  <li>Definition lists
	  </ol>
	  as well as simple structures.
	  <p>Markup minimization (later generalized and formalized in SGML),
	  allowed the end-tags to be omitted for the "h1" and "p" elements.

^
* SGML incorporated same "tags" but used angle bracket notation instead
* This is the same text marked up with SGML instead of GML
* [Flip back and forth]

----

## HTML (HyperText Markup Language)

	  <h1>Chapter 1: Introduction</h1>
	  <p>GML supported hierarchical containers, such as
	  <ol>
	  <li>Ordered lists (like this one),
	  <li>Unordered lists, and
	  <li>Definition lists
	  </ol>
	  as well as simple structures.
	  <p>Markup minimization (later generalized and formalized in SGML),
	  allowed the end-tags to be omitted for the "h1" and "p" elements.

^
* HTML directly absorbed SGML: identical notation
* [Flip back] Exact same markup
* HTML simplified SGML greatly
* SGML: describe structure of complex documents
* HTML: present Web pages in browser

----

## HTML hyperlinks

	   <a href="http://digstud.bitfragment.net">Link to course syllabus site</a>

^
* HTML added a feature not found in SGML, for its new function in Web browser
* [Explain syntax]
* [Demo any hyperlink on course syllabus site]
* These pages are written in HTML markup
* [View source in Chrome + enlarge text; flip back and forth]

----

## Tryit Editor v2.0

^
* [Open and demo]
* "Here is some text. I can emphasize text, or place it in bold face. I can make a link to the course syllabus Web site."

----

## SGML (1980; primarily semantic or *descriptive* markup) → 
## HTML (1990s; *presentation* markup)

^
* HTML's history as a presentation markup format:
* Absorbed SGML, designed as semantic markup
* SGML in turn had been based on GML, a processing markup
* A certain tension evolved from this history

----

## Description of a text's structure

    <h1>A level 1 section heading</h1>
    
    <p>A paragraph</p>
    
## Presentation of styled or "rich" text

    <i>Italicized text</i>
    
    <b>Boldface text</b>

^
* In early HTML, there was a tension
* Between the descriptive elements of SGML: what this is
* And elements needed most often for *presenting* text on a screen: how it looks

----

## Mixing structure and presentation

    <h1>A level 1 section heading 
    with some <i>italicized text</i> in it</h1>
^
* Web designers often mixed them together
* [Explain]

----

## Mixing structure and presentation

    <h1>A level 1 section heading with some 
    <i><font color="red">italicized 
    and colored text</font></i> 
    in it</h1>

^
* And this could make the code look very complicated
* But also confusing: two different purposes
* [Demo this in Tryit Editor]
* [h1 and a p]
* [add italic text inside h1]
* [add 2 different colored text inside italicized, using '<font color="x">'

----

## Separation of content (structure) and form (style)

![inline,left](http://localvox.com/wp-content/uploads/2013/03/bold-italics1.jpg)

![inline,right,200%](http://farm8.staticflickr.com/7077/7164254600_4869a4fb68.jpg)

^
* Early webdevs: these two things shouldn't be mingled
* Section/paragraph = structural element, doesn't change
* Color, italics, bold, etc. = context-dependent
* Different colors, forms of emphasis, etc. used in different languages and typesetting styles
* E.g., German *Sperrsatz*
* Didn't want to have to rewrite HTML using different forms of emphasis

----

## HTML today: the front-end Web development “stack”

1. HTML
2. **CSS** (Cascading Style Sheets)

^
* CSS = style language to be used along with HTML markup format
* Moves presentation instructions into a separate section of the HTML code, or event a separate document, called the style sheets

----

## HTML

	    <h1>A level 1 section heading</h1>
    
## CSS

	    h1 { 
	    	font-size: 24pt;
	    	font-color: red;
	    	}

----

## CSSDesk.com

^
* [Open and demonstrate the html/css on the previous slide]
* Now HTML describes the structural elements of the document
* CSS controls its presentation

----

## Internal style sheets

	   <style>
	       h1 { 
	    	font-size: 24pt;
	    	font-color: red;
	    	}
	   </style>

^
* CSS can be incorporated into the HTML markup of a document
* Between a set of special tags

----

## External style sheets

	   <link rel="stylesheet" type="text/css" href="mystyle.css">

^
* These days, CSS is sophisticated enough so that usually external
* You can view it along with HTML source in a browser
* [Show them using course syllabus Web site]

----

## HTML today: the front-end Web development “stack”

1. HTML
2. CSS (Cascading Style Sheets)
3. **JavaScript**

^
* There is a third element of the stack
* Special-purpose programming language
* Developed along with HTML and CSS for programming inside a Web page

----

## JavaScript

		<script> 
			document.write("Hello World!);
		</script>

^
* It's a proglang, which is our next unit, so just a bit here
* Language is contained in the browser: Safari, Chrome, Firefox
* Like CSS, can be incorporated into HTML markup of a document…
* …or JavaScript files can be linked
* [Show them using psu.edu]

----

## JavaScript in your browser

^
* You can access it if you want to
* [Demo on Chrome: alert, document.write]

----

## Client-side scripting (JavaScript)
## Server-side scripting (PHP)

^
* There is one more programming language used inside HTML markup: PHP
* JavaScript is executed in browser: client-side
* Your browser is the client
* PHP is executed on the server side

----

## PHP
		
		<?php
		 echo "Hello World!";
		?>

^
* [Open compileonline.com for PHP]
* [Add h1 header text]
* [Add paragraph]
* [Then add PHP hello world]
