# Website Update Instructions for Al-folio

Before making any changes, make sure to run this command. 
```
git pull origin main
```
Running this command allows you to get the most recent change to your repository.


After that, you can make any of the changes I have highlighted below.

After making the necessary changes, Run the following commands to push and deploy your changes. 
``` 
git add . 
git commit -m "A description or message of what you did" 
git push 
``` 

## Add a publication
To add a new publication to the website, add a new entry to the `_bibliography/papers.bib` file. 

Here is an example entry: 
```
@article{chong_global_2021,
	abbr = {Taylor & Francis},
	arxiv = {2008.01753},
	author = {Jacky J. Chong and Manoussos G. Grillakis and Matei Machedon and Zehua Zhao},
	journal = {Communications in Partial Differential Equations,},
	journal_link = {https://www.tandfonline.com/doi/abs/10.1080/03605302.2021.1920615?journalCode=lpde20},
	title = {Global Estimates for the Hartree--Fock--Bogoliubov Equations},
	year = {2021}}
```
`chong_global_2021` is a variable name for this article, and the variable name can be anything with no spaces or weird punctuations. 

## Adding a news
To add a new news on the website, create a new .md file in the `_news/` folder. Name of the file is just a variable name. 

Here is an example of a non-hyperlinked news: 

SNU_talk.md
```
---
layout: post
title: Seoul National University, Analysis Seminar
date: 2022-10-12
inline: true
hide: false
---

Seoul National University, Analysis Seminar
```

`inline`: setting this variable to true makes the post non hyperlinked. Only the `title` of the news appear on the website. Setting this to false make the post hyperlinked, and when pressing the hyperlink, the website will redirect users to a new page showing everything below the second "---" in the file. 

`hide`: Setting this to true hides the news in the website. Alternatively, you can just delete the news .md file.

