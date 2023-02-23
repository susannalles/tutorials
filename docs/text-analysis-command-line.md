---
layout: default
title: Text Analysis with Command Line
date:   2023
author: Susanna Allés Torrent
nav_order: 7
---

Some basic tasks of text analysis can be performed through the command line. 

- Install [Wget](https://www.gnu.org/software/wget/) 
- Place yourself in your working directory (e.g. /Users/susername/Documents/DHPracticum)
- Download any text, e.g. `wget http://archive.org/download/thestoriesmother05792gut/stmtn10.txt
ls`
- Check the file is there: `ls`
- Get the information about that file: `file stmtn10.txt`
- Get the first few lines of the file: `head stmtn10.txt`
- Get the last few lines of the file: `tail stmtn10.txt`
- Copy the file to make a backup: `cp stmtn10.txt stmtn10-backup.txt` and check the new file is there: `ls`. 
- Have a look to the whole file: `less -N stmtn10.txt`
- To look for a word: `/giant`, to find the next occurence `n`, and to leave the file `q`. 
- Remove the final lines of the documents: `sed '2206,2525d' stmtn10.txt > stmtn10-nofooter.txt`
- Remove lines from 1 to 40: `sed '1,40d' stmtn10-nofooter.txt > stmtn10-trimmed.txt`
- Check you have all the created files with `ls`
- Count the lines of the file: `wc -l stmtn10-trimmed.txt`
- Count the characters of the file: `wc -m stmtn10-trimmed.txt`
- Get the line number where a word appears: `grep -n "giant" stmtn10-trimmed.txt`
- Find pattern (-E) and get line numbers (-n) looking for lowercase and capital letter: `grep -E -n "(G|g)iant" stmtn10-trimmed.txt`
- Standarize the text by removing the punctuation of the file: `tr -d '[:punct:]' < stmtn10-trimmed.txt > stmtn10-nopunct.txt`
- And by removing capital letters: `tr '[:upper:]' '[:lower:]' < stmtn10-nopunct.txt > stmtn10-lowercase.txt`
- Normalize the carriage returns: `tr -d '\r' < stmtn10-lowercase.txt > stmtn10-lowercaself.txt`
- Transform each blank space into an end-of-line character: `tr ' ' '\n' < stmtn10-lowercaself.txt > stmtn10-oneword.txt`
- Sort words alphabetically: `sort stmtn10-oneword.txt > stmtn10-onewordsort.txt`
- Create a new file where the words are listed alphabetically, each preceded by its frequency: `uniq -c stmtn10-onewordsort.txt > stmtn10-wordfreq.txt`
- Check the beginning of the file: `head stmtn10-wordfreq.txt`
- Create a pipeline instead of several files: `tr ' ' '\n' < stmtn10-lowercaself.txt | sort | uniq -c > stmtn10-wordfreq2.txt`

This commands were taken from: William J Turkel (2013). [Basic Text Analysis with Command Line Tools in Linux](https://williamjturkel.net/2013/06/15/basic-text-analysis-with-command-line-tools-in-linux/)


