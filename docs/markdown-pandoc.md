---
layout: default
title: Markdown
nav_order: 1
---

# What you need to work today?

- A plain text editor (Mac, Linux, Windows): [VS Code](https://code.visualstudio.com/)
- Command Line
  * Mac: cmd+space, type "terminal"
  * Windows: hit Super/Windows key, type "powershell" and press Enter
- [Pandoc](https://pandoc.org/installing.html) to convert to different files.
- Some latex version to create pdf files
    - [Miktex](https://miktex.org/) works on Mac, Linux and Windows.
    - On Mac, [basictex](www.tug.org/mactex/morepackages.html) also worked fine.
- Online alternative: <https://dillinger.io/>
- Download this [file](http://susannalles.com/markdown.zip)

# What is Markdown?

- .md is a markup language that you can use to add formatting elements to plaintext documents.
- one of the world’s most popular markup languages
- it only care for writing, not formatting (WYSIWYG)
- it is light enough to read it in naked eye
- you can use any text editor application

# Why to use Markdown

- Markdown can be used for everything: create websites, documents, notes, books, presentations, email messages, or technical documentation.
- Markdown is portable, you can use any application (open-access) (vs Microsoft Word is a proprietary file format)
- Markdown is platform independent (any operating system)
- Markdown is used worldwide and it is used for websites like Reddit or GitHub.
- Markdown is a fast and easy way to take notes, create content for a website, and produce print-ready documents.

# Why not Microsoft Word or Google Drive?

- Word seems easy now, but it will drive you crazy in the long run.
- Microsoft Office package is expensive.
- Files are not universal.
- Word is very distractive.
- Problems with incompatibility.
- Files are heavier and tend to corrupt.
- Problems merging files, copying text from other files, numbering.

[RafaDavis](https://github.com/rafadavis/markdown-workshop/blob/master/README.md)

# Why should I use Markdown?

- Beautiful professional formatting without much work.
- It can easily be converted to other formats: doc, pdf, html, etc.
- Separation of form and content allows you to focus on your writing.
- Text editors are meant to be worked with text structure, so they force you to think about the organization of your writing.
- Future proofing your files: plain text files are universal. They will work on any computer, of any operational system, forever.
- There is no lock-in. If you don't like it, you can convert the files to doc files and go back to work the way you used to.
- The more you learn, the more powerful tools you can access, such as automatic citations.
- If you are writing a dissertation, or a thesis, there is a good chance your university has the template ready, so you don't need to worry about adjusting to their standards.

[RafaDavis](https://github.com/rafadavis/markdown-workshop/blob/master/README.md)

# You even can create Websites

- Jekyll https://www.markdownguide.org/tools/jekyll/
- Blot: https://blot.im/
- Small Victory:  https://www.smallvictori.es/
- Other static web generators https://jamstack.org/generators/

# The basics

Check this https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf

# Exercice 1: Create a Markdown file

A Markdow file is nothing more than a text file, saved with the extension ".md".

- Open the file test.md
- Edit it as you like taking some elements from the Cheatsheet Markdown Syntax
- Save it


# Now, how do we transform this?

- There are different ways to transform .md into other formats.
- The most common is Pandoc: a collection of parsers and scripts that transform a plain text file in .md into HTML, PDF, doc, Slides, etc.
-  We will use the terminal
  * Mac: press *CMD + Space*, type "terminal" and press *Enter*
  * Windows: hit *Super/Windows* key, type "powershell" and press Enter

# Basic commands for the terminal

- `pwd`: Present working directory
- `ls`: List Directory
- `mkdir`: Make Directory
- `cd`: Change Directory
- `cd ..`: Change to parent directory

Type:

- `cd Documents`
- `mkdir MarkdownWorkshop`
- `cd MarkdownWorkshop`

# Pandoc

- You had to install [Pandoc](https://github.com/jgm/pandoc/releases/tag/2.3.1) to convert to different files.
- Some latex version to create pdf files
    - [Miktex](https://miktex.org/) works on Mac, Linux and Windows.
    - On mac, [basictex](www.tug.org/mactex/morepackages.html) also worked fine.
- If Pandoc or Latex is not correctly installed, this will not work

# Exercice 2: Transformation

- Go to your terminal (you should be there already but it you are not type `pwd` and `cd` to our folder "MarkdownWorkshop")
- Type simply: `pandoc test.md -o test.pdf`
- Go to you folder and check the new PDF

# Exercice 3: Open test2.md

- Explore this document and try to transform it from the terminal: `pandoc test2.md -o test2.pdf`
- To create other types of documents, you only need to change the extension. For instance, if you want a Word doc, type "pandoc -o test2.docx test.md". Same goes for ".html", ".odt", etc.
- Into a HTML: `pandoc test2.md -o test2.html`
- Into a Doc: `pandoc test2.md -o test2.odt`
- YAML metadata

# And what about your disseration?

There are a lot of templates out there you can use:

- Template for U Oxford: https://github.com/tompollard/phd_thesis_markdown
- markdown-paper: https://github.com/ihrke/markdown-paper/tree/master/pdf
- Overleaf: https://es.overleaf.com/gallery/tagged/markup

# Eisvogel Template

- https://github.com/Wandmalfarbe/pandoc-latex-template
- https://tthub.io/aprende/l1-intro-a-tei/
- https://zenodo.org/record/4430863#.YDWABmMo_L8
