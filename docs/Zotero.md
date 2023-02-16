---
layout: default
title: Zotero
date:   2018-09-24
author: Susanna Allés Torrent
nav_order: 3
---

# What is Zotero? 

Zotero is a citation managment tool. It is free and multiplatform (Windows, Linux, Mac).  

The last version, Zotero 5.0, is used as an standalone software on your machine and as a Firefox extension (It can be used with Chrome and Safari but the plugin extension is not completely developed).  

Zotero helps you to "collect, organize, cite, and share research". 


# Step 1: Create username and install Firefox connector

- Download and Install [Firefox](https://www.mozilla.org/en-US/firefox/new/), if you don't have it. I recommend you to use this browser instead of Edge, for example. 
- Create a username in Zotero: <https://www.zotero.org/user/register>

![Image](img/zotero_03.png)

Once you are logged in, you can manage your folders and all your items: 

![Image](img/zotero_04.png)

At this point, you can try to create a folder collection realted to this course or to your disseration. 

## Sept 2: Download Zotero

The best way to use Zotero is an standalone app, as such you can use it even if you don't have an internet connection: 

- [Download Zotero 5.0](https://www.zotero.org/download/)

![Image](img/zotero_01.png)

Now, you have to download the Firefox Connector to be able to collect all items that you need for your bibliography: 

- [Download Zotero Firefox Connector](https://www.zotero.org/download/) 

![Image](img/zotero_02.png)

Once you have install the connector you will need to restart your browser, and you will see a litle icon on the top right corner that indicate the type of document that the browser is displaying: 

![Image](img/zotero_05.png)
![Image](img/zotero_06.png)
![Image](img/zotero_07.png)
![Image](img/zotero_08.png)

Open your Zotero app, login with your credentials, and start exporting articles, books, etc. that you whish. 

## Step 3: Syncornization with your Zotero account 

Zotero is syncronized with your app and with the online platform. Be sure at the very begining that you login with your credentials, at Zotero > Prefernces 

![Image](img/zotero_09.png)

If sometimes you need to syncronize it faster or be sure that everything is up to date, click the sync botton in the top right corner of your app:

![Image](img/zotero_10.png) 

## Step 4: Create a Collection 

You can create collections from the online platform or from your app, by clicking in this icon:
 
![Image](img/zotero_11.png)

## Step 5: Collect bibliographical items

Go to UM catalog library and find some bibliography you need <https://www.library.miami.edu/>. 

- Download at least 4.  
- Visualize in the list: title, Creator, Item Type, Date 
- Explore the Metadata section: Infos, Notes, Tags, Related 

## Step 6: Add notes, and tags 

For each item, you can add personal notes, and also tags or keywords. 

![Image](img/zotero_13.png)

![Image](img/zotero_14.png)

## Step 7: Collaborate and share bibliography 

To create a Group collection that will be shared with other people: 

![Image](img/zotero_12.png)


## Step 7: Export in different citation styles 

Choose the items you want in your bibliography 

![Image](img/zotero_15.png)

Choose the style you want (MLA, Chicago, etc.): 

![Image](img/zotero_16.png)

Save it in rdf format or docx or pdf: 

![Image](img/zotero_17.png)

And voilà: 

![Image](img/zotero_18.png)

## Step 8: Export it directly to Microsoft and LiberOffice

Last versions of Microsoft Word have the Zotero plugin installed automatically when you install the app. So it is easy as open Word after the installation and you have it: 

![Image](img/zotero_19.png)

While you write, you can add and edit citations in your text. 

![Image](img/zotero_20.png)

For which, a pop-up windwow will appear with all your items:

![Image](img/zotero_21.png)

And at the end you can create the full bibliography which will be created with the items that you have cited. 

![Image](img/zotero_22.png)

## Timelines

You can create a timeline of your bibliography, going to Tools > Create Timeline: 

![Image](img/zotero_23.png)

## And the coolest thing: Zotero API 

You can do many things with the API, one of which is to import your bibliography directly to your webpage with a line of code: 

```html
h2>Diachronic Spanish Corpus Linguistics</h2>

<?php $URL='https://api.zotero.org/users/1167759/collections/GCNLKMRQ/items?format=bib&style=chicago-author-date'; $var=file_get_contents($URL); echo $var?>
	
</div>
```

![Image](img/zotero_24.png)


