![100%](http://img.xataka.com/2013/10/bit-0-1.jpg)

^
* "Bit" is in many ways entirely abstract
* We can't even see most of its representations

----

![inline,left,100%](http://isis.astrogeology.usgs.gov/IsisWorkshop/uploads/0/0d/Bit-byte-word.jpg)

![inline,right,150%](http://seemisadia.files.wordpress.com/2013/06/words.jpg)

^
* In memory addressing, the concepts of word and word size are adapted from the domain of natural (human) language

----

![fit](http://ecx.images-amazon.com/images/I/61tdpgruLeL._SL1500_.jpg)

^
* The concept of the file is considerably less abstract
* We have a concept of a file as something concrete, at least

----

![100%](http://i.i.cbsi.com/cnwk.1d/i/tim/2012/08/20/iCloudDocuments.png)

^
* The virtual space of our operating systems…
* …provide us with a similarly tangible concept of a file as an object resting on a "desktop" surface

----

![fit](http://www.wired.com/images_blogs/gadgetlab/2013/04/Messy_desktop.png)

^
Just like your real desktop, your virtual desktop can get very cluttered with such objects

----

![125%](http://joedale.typepad.com/photos/uncategorized/electronic_filing_hg_wht_23285.gif)

^ 
* But how do those files get in there?
* Obviously, we don't toss files into the computer as we might in to a recycling bin
* This is a visual metaphor for conversion to digital representation

----

![fit](http://3.bp.blogspot.com/_UElib2WLeDE/TKOkWuJhDLI/AAAAAAAACV0/J7U4Z-ee4tc/s1600/binary.jpg)

^
* What to you is represented as a file sitting on your "desktop" is to your computer…
* …just another sequence of ones and zeroes
* a particular *group* of sequences of ones and zeroes

----

![fit](https://openclipart.org/image/2400px/svg_to_png/149755/Binary_file-20110715.png)

^
* This means that even though unlike the bit, the file is represented for us in a familiar form…
* …the digital genre of the "file" is fundamentally an abstraction as well
* A linear array (indexed sequence) of bytes stored on a durable medium

----

![fit](http://upload.wikimedia.org/wikipedia/commons/2/2c/Hexedit-screenshot.png)

^
* How is data stored in a file?
* In binary encoding, like everything else
* Here, hex notation for the binary encoding of an ASCII text file

----

## Viewing hex and binary representation of data in an ASCII text file

^
[Using Javascript PC emulator or your own terminal]
* explain GUI vs CLI
* echo ‘hello’ >  temp/hello.txt
* show them and quicklook the file in finder.app
* hexdump foo.txt
* hexdump -C
* xxd -b

----

![fit](http://www.hdsentinel.com/img/cases/img_65_hddsurface4.gif)

^
* Your file is stored on a storage medium, e.g., hard disk
* How does the OS keep track of files?
* Memory addressing: numbering their locations, just like houses on a street
* Units of memory addressing: 'blocks' and 'pages'

----

![fit](https://cdn.tutsplus.com/mac/uploads/2014/01/TRIM-ExplanationOff-1.jpg)

^
* Blocks have a certain size
* A file can be (almost always is) distributed over multiple blocks
* [Explain image]
* Files are not discrete objects, as they seem on desktop
* They are simply the boundaries of groupings of blocks of data

----

## Elements of a file

1. Identifier: memory address plus file attribute metadata
2. Name (given by user or by OS)
3. Contents

^
* File attribute metadata: modification date, owner, access permissions, etc.

---

## Viewing file elements

^
[Using Javascript PC emulator or your own terminal]
* use foo.txt from earlier example
* file identifier + name: `ls -li foo.txt`
* file contents: `cat foo.txt`
* [do `ls` and `cat` once more]

----

![175%](http://2.bp.blogspot.com/-8CjZ-HV3QrE/T53tg47YVxI/AAAAAAAAANA/8gfG89Wiy48/s1600/onof.png)

^
* Data in the file I just created is binary data
* All data stored or transmitted by a computer is binary data
* Text, images, audio and video, and compiled executable program files
* Machine-readable; not human-readable

----

![150%](http://math2033.uark.edu/wiki/images/thumb/5/57/Binaryscarf.jpeg/500px-Binaryscarf.jpeg)

^
In complex form like a file, those forms of data consist of sequences of alternation between two states

----

![fit](http://rus-linux.net/MyLDP/BOOKS/drivers/DD-2-xxd-showing-initial-data-on-first-partition.png)

^
* Text data is binary data that happens to be represented as text…
* So as to be human-readable, for human purposes

----

![100%](http://icongal.com/gallery/image/9172/document_text_file_txt.png)

^
* Text file as container of the content *text data*
* Most of the text files you use, you use for writing and reading

----

![100%](http://www.edwardtufte.com/bboard/images/0003l6-9855.jpg)

^
* A computer program is a special kind of text file
* It can be compiled and then executed
* [create hello.c]
* cat hello.c
* gcc hello.c
* hexdump a.out
* hexdump -C a.out

----

## Filesystem elements

1. File
2. Directory
3. Metadata

^
* [show them hello.txt in its folder]

----

![fit](http://i.stack.imgur.com/r7Ahq.png)

^
* Like the file, the file system presents us with a visual analogy derived from the domain of paper documents
* Abstract groupings, called directories, for the abstract objects we call files
* Image: representation of a hierarchical file system for an early computer…
* …as labeled folders inside an enclosing folder

----

![fit](http://etc-mysitemyway.s3.amazonaws.com/icons/legacy-previews/icons/glossy-black-icons-business/080774-glossy-black-icon-business-folder2-sc1.png)

^
A folder icon is a graphical user interface metaphor that represents the directory as a container into which we can place files

----

## History of filesystem design

* Vannevar Bush, memex
* Douglas Engelbart, NLS
* Ted Nelson, Xanadu/ "dream file"
* Unix

----

![fit](https://www.youtube.com/watch?v=c539cK58ees)

^
* Vannevar Bush, 1945: concept of an electromechanical filesystem…
* …that allows one to build associative trails linking materials
* …via metadata attributes (memory addresses) that the device keeps track of for you

----

## Vannevar Bush, "As We May Think" (1945)

* Social benefits of science
* Conditions of modern progress
* Problems with specialization
* “A transformation in scientific records”

^
* V.B. was not just an inventor tinkering with a design for a gadget
* One of the great engineer-intellectuals of the WWII era
* Big questions of science, technology, war and peace
* ?(Why) [atomic warfare and crisis of ethics, replacement of God]
* Essay has an intellectual agenda
* Four issues addressed in essay on memex [review slide]

----

## Vannevar Bush, "As We May Think" (1945)

* Social benefits of science
	1. Material: food, clothing, shelter, physical health
	1. Immaterial: knowledge

----

## Vannevar Bush, "As We May Think" (1945)

* Conditions of modern progress
	1. Knowledge requires specialization
	1. Specialization is necessary for progress

----

## Vannevar Bush, "As We May Think" (1945)

* Problems with specialization
	1. Fragments knowledge
	1. Produces knowledge in excess

----

## Vannevar Bush, "As We May Think" (1945)

* “A transformation in scientific records”
	1. “Mechanical aids”
	1. “Mature,” “creative” thought

^
* We can use filesystem designs like the memex as mechanical aids…
* To do the routine work of managing files for us
* …freeing us to engage in 'mature,' 'creative' thought

----

## Vannevar Bush, "As We May Think" (1945)

Indexing systems: arbitrary linear sequences

* 1, 2, 3, 4, 5, 6, 7, 8, 9, 10…
* A, B, C, D, E, F, G, H, I, J, K, L…

> “The human mind does not work that way. [Rather,] It operates by association

^
* The linear sequences of our traditional indexing systems are too rigid
* They are mechanical, which is why a filesystem can handle them efficiently for us
* Human thought operates not by arranging things in linear order, but by making associations between them

----

## Vannevar Bush, "As We May Think" (1945)

Associative, rather than linear indexing

> This is the essential feature of the memex

^
* As a labor-saving filesystem design that frees us for mature, creative thought

----

## Douglas Engelbart, NLS (“oN Line System”) demo (1968)

* Clip #2, introduction
* Clip #3, Word processing and file creation

^
* December 9, 1968 public demo of NLS, another early filesystem design
* Augmentation Research Center, Stanford Research Institute, Menlo Park
* Early versions hardware we use today: most famously, mouse
* Early versions of OS, filesystem software as we recognize it today
* [Watch 2 clips]

----

## Ted Nelson, "A File Structure for the Complex, the Changing and the Indeterminate" (1965)

* Personal use of computer vs. business/ scientific data processing

> The kinds of file structures required if we are to use the computer for personal files and as an adjunct to creativity are wholly different in character from those customary in business and scientific data processing

^
* Bush was concerned with professional academic and corporate research
* Nelson focused on everyday consumer and creative use of a filesystem

----

## Ted Nelson, "A File Structure for the Complex, the Changing and the Indeterminate" (1965)

> …the dream file: the file system that would have every feature a novelist or absent-minded professor could want, holding everything he wanted in just the complicated way he wanted it held, and handling notes and manuscripts in as subtle and complex ways as he wanted them handled

^
* Nelson really did mean creative: for example, a "novelist or absent-minded professor"
* Otherwise goal is similar to memex: let filesystem handle managing materials…
* …and free the human being for creativity

----

## Ted Nelson, "A File Structure for the Complex, the Changing and the Indeterminate" (1965)

> The physical universe is not all that decays. So do abstractions and categories. Human ideas, scholarship, and language are constantly collapsing and unfolding. … While [this process] may be erratic, it never stops; and the meaning of all this for information retrieval should be clear

^
* Here, too, not about gadgets, but a philosophical argument about time and change
* ?(What's 'the meaning of all this for information retrieval') -> [1 minute; discuss]

----

## Ted Nelson, "A File Structure for the Complex, the Changing and the Indeterminate" (1965)

> To the extent that information retrieval is concerned with seeking *true* or *ideal* or *permanent* codes and categories… [it] seems to me to be fundamentally mistaken. *The* categories are chimerical (or temporal) and our categorization systems must evolve as they do. … [T]he only ultimate structure is change itself

^
* Using a machine to help us cope with time and change
* Using it as a creative tool

----

## Filesystems; early history

Big ideas; mundane or prosaic implementations
