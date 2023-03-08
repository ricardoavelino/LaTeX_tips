# Tips on LaTeX thesis writing
Author: @ricardoavelino

Hello, I prepared this guide to share how I set up my thesis writing with LaTeX + VSCode + Zotero. I hope it helps. But remember, the best way is always your way.

1)	Download VSCode + LaTeX extension

Since long, I have been using VSCode to code with Python and I decided to keep the same IDE for the thesis writing.

-	https://code.visualstudio.com 

Compiling LaTeX files in VSCode is easier since version 1.74. Make sure you have VSCode’s newest version and download the extension called “LaTeX Workshop” from James Yu.

 

His extension is maintained through this repo. If you have issues, you can look at the issue tracker and/or open your own:

-	https://github.com/James-Yu/LaTeX-Workshop 

To compile the LaTeX files, you can go to the “TeX” icon on the left bar and click on Build LaTeX Project and the document will be created, looking like the following:

 

2)	Other helpful extensions at VS Code:

-	LaTeX Utilities: Help out to create shortcuts for copying and pasting stuff. For example, with this extension you can copy a table in excel and it becomes a table with LaTeX code. Also help on writing equations in LaTeX.

https://marketplace.visualstudio.com/items?itemName=tecosaur.latex-utilities

-	Grammarly extension: Grammar checking extension which works quite fairly, even in the middle of LaTeX code. It works well also if you have Grammarly Premium since it can connect to your account over VSCode. Make sure you also configure the language, e.g. English British, and check the correction settings. There are other grammar checking extensions if you don’t like Grammarly. Make sure you have one!

https://marketplace.visualstudio.com/items?itemName=znck.grammarly 

3)	Managing citations with Zotero:

For managing citations, I have been using Zotero (thanks to @selina). It requires a good amount of commitment and it will not be perfect right away. Many citations come wrong and it is a time-consuming process to edit all of them, but it pays off at the end…

-	https://www.zotero.org 

My library at Zotero looks like this 

 
You can adjust citations by directly clicking on them and editing any detail that is wrong.

Make sure you install Zotero extensions to your browser, this way it is easier to import information about articles directly from the article page. For example, on the top left the icon “Save to Zotero” will import the information to your library (not always work).

 

Keep your library clean as it will then help you to writing future articles, etc… Try to start early.

4)	Zotero citation export:

Now that you have a clean library of references in Zotero you want to set up a live export of this citations to a .bib file. This means that every time you read a new paper, and add it to your Zotero library, this will update the .bib file at your thesis/article. 

To achieve that, first download and install Zotero’s extension Better BibTeX: 

-	https://retorque.re/zotero-better-bibtex/ 

This extension eases the automatic export process. Once it is installed go ahead and export your library in Zotero > Export Library > Format: Better BibTeX > [x] Background Export > OK. As in the image below. 

 
You can save the .bib within your thesis folder and link your references to it in LaTeX. If you are unsure how to do the LaTeX part make sure you read about it in the MULTIPLE LaTeX tutorials available online, for example here:

-	https://www.overleaf.com/learn/latex/Bibliography_management_with_bibtex 

For example, I exported my Zotero library to a file called references.bib within my Thesis folder. The citations will be automatically updated in this file if you make any modification, e.g., a correction in a citation that you imported wrongly. 

 

You can browse through some other cool Zotero extensions, I HIGHLY suggest that you use the Better BibTeX function to “standardize” all citation keys. I standardized all my citations as [AUTHOR LAST NAME]_[PAPER FIRST WORD]_[YEAR]. If you do that, Better BibTeX will overwrite all the citation keys that you import to this format and it will help you to cite them at your document afterwards. For example.

\cite{livesley_computational_1992} 

Also, the autocomplete functions of VSCode should work fairly well, so when you start typing the name of the author, you should get the options for citing the papers from that author.

5)	Create a repository to store your thesis as you write it:

To back up your document and keep track of your writing progress, I also suggest that you create a repository at GitHub to store your thesis and commit to it often.

 
You can use any Git manager to do that. I have been using GitKraken

-	https://www.gitkraken.com 





