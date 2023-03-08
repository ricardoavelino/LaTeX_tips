# Tips on LaTeX thesis writing

Hello, I prepared this guide to share how I set up my thesis writing with LaTeX + VSCode + Zotero. I hope it helps. But remember, the best way is always your way.

## 1.	Download VSCode + LaTeX Wokshop

Since long, I have been using [VSCode](https://github.com/microsoft/vscode) to code with Python and I decided to keep the same IDE for the thesis writing.

-	https://code.visualstudio.com

Compiling LaTeX files in VSCode is easier since version ``1.74``. Make sure you have VSCode’s newest version and download the extension called [LaTeX Workshop](https://github.com/James-Yu/LaTeX-Workshop) from [James Yu](https://github.com/James-Yu).

<img width="1352" alt="image" src="https://user-images.githubusercontent.com/36137188/223685322-b3e80fb7-95d9-4390-8dfe-05374938b94e.png">

His extension is maintained through the following repository. If you have issues, you can look at the issue tracker and/or open your own:

-	https://github.com/James-Yu/LaTeX-Workshop 

To compile the LaTeX files, you can go to the ``TeX`` icon on the left bar and click on Build LaTeX Project and the document will be created, looking like the following:

<img width="1680" alt="image" src="https://user-images.githubusercontent.com/36137188/223686887-86a08846-d70c-402d-93b0-bc058b5b5d43.png">

## 2.	Other helpful extensions at VSCode:

- __LaTeX Utilities__: Help to create shortcuts for copying and pasting stuff. For example, with this extension you can copy a table in excel and it becomes a table with LaTeX code. Or even a .png image with the necessary syntax to add the figure in LaTex. Also help on writing equations etc.

- https://marketplace.visualstudio.com/items?itemName=tecosaur.latex-utilities

-	__Grammarly extension__: Grammar checking extension which works well, even in the middle of LaTeX code. If you have Grammarly Premium you can also connect to your account via VSCode and get better suggestions. Make sure you also configure the language, e.g. English American/British and writing style. There are other grammar checking extensions if you don’t like Grammarly. Make sure you have one!

- https://marketplace.visualstudio.com/items?itemName=znck.grammarly 

## 3.	Managing citations with Zotero:

For managing citations, I have been using [Zotero](https://www.zotero.org). It requires a good amount of commitment and it will not be perfect right away. Many citations come wrong and it is a time-consuming process to edit all of them, but it pays off at the end…

-	https://www.zotero.org 

My library at Zotero looks like this:

<img width="1550" alt="image" src="https://user-images.githubusercontent.com/36137188/223688139-19f9142f-906a-4cea-9f96-b068a709d3c4.png">

You can adjust citations by directly clicking on them and editing any detail that might be wrong.

Make sure you install Zotero extensions to your browser, this way it is easier to import information about articles directly from the article page. For example, on the top left the icon _Save to Zotero_ will import the information to your library (always double check!).

<img width="1792" alt="image" src="https://user-images.githubusercontent.com/36137188/223688399-7ebee5e7-a00c-459c-9178-1896a241abe9.png">

Keep your library clean as it will then help you to writing future articles, etc… Try to start early.

## 4. Zotero citation export:

Now that you have a clean library of references in Zotero you want to set up a live export of this citations to a ``.bib`` file. This means that every time you read a new paper, and add it to your Zotero library, this will update the ``.bib`` file at your thesis/article. 

To achieve that, first download and install Zotero’s extension [Better BibTeX](https://retorque.re/zotero-better-bibtex/): 

-	https://retorque.re/zotero-better-bibtex/ 

This extension eases the automatic export process. Once it is installed go ahead and export your library with

- _Zotero > Export Library > Format: Better BibTeX > [x] Background Export | [x] Keep Updated > OK_. As in the image below:

<img width="1550" alt="image" src="https://user-images.githubusercontent.com/36137188/223689204-58fb4da4-c16b-471f-81bc-e443c02546e0.png">
 
You can save the ``.bib`` within your thesis folder and link your references to it in LaTeX. If you are unsure how to do the LaTeX part, make sure you read about it in the multiple LaTeX tutorials available online, such as the Overleaf tutorial, see here:

-	https://www.overleaf.com/learn/latex/Bibliography_management_with_bibtex 

For example, I exported my Zotero library to a file called references.bib within my Thesis folder. The citations will be automatically updated in this file if you make any modification, e.g., a correction in a citation that you imported wrongly. 

<img width="1792" alt="image" src="https://user-images.githubusercontent.com/36137188/223689620-57134d3c-b536-4968-a283-e1d2366910c3.png">

You can browse through some other cool Zotero extensions, I highly suggest that you use the Better BibTeX function to standardize all citation keys (see the docs). I standardized all my citations as _[AUTHOR]_[PAPER FIRST WORD]_[YEAR]_. If you do that, Better BibTeX will overwrite all the citation keys that you import to this format and it will help you to cite them at your document afterwards. For example.
```
\cite{livesley_computational_1992} 
```
Also, the autocomplete functions of VSCode should work fairly well, so when you start typing the name of the author, you should get the options for citing the papers from that author.

## 5.	Create a repository to store your thesis as you write it:

To back up your document and keep track of your writing progress, I also suggest that you create a repository at GitHub to store your thesis and commit to it as you go.

<img width="909" alt="image" src="https://user-images.githubusercontent.com/36137188/223690366-74f79a6c-5cc6-45dc-b5e0-4174313389b0.png">

You can use any Git manager to do that. I have been using GitKraken

-	https://www.gitkraken.com

## 6.	Download template:

Regarding the organization of the documment I have organized my _chapters, figures and extra pages_ in separate folders. The main file of the thesis: ``phd.tex`` only calls these files. The template is uploaded in this repository and it has been a cummulative work of many including:

- [Matthias Rippmann](https://block.arch.ethz.ch/brg/people/matthias-rippmann)
- [Robin Oval](https://block.arch.ethz.ch/brg/people/robin-oval)
- [Ricardo Avelino](https://block.arch.ethz.ch/brg/people/ricardo-maia-avelino)
- [Gene Kao](https://block.arch.ethz.ch/brg/people/gene-ting-chun-kao)

Have a fun writing.
