+++
title = "My Writing Flow"
date = "2021-03-04T07:25:52Z"
author = "Josh Cain"
authorTwitter = "kmartkart" #do not include @
cover = ""
tags = ["flow", "tex", "org", "markdown"]
keywords = ["", ""]
description = "A certain way I do things"
showFullContent = false
+++

## Introduction

I'm wanting to share my own writing workflow with you all, just something I think that many of you might find interesting.

I'm a fan of Open Source Software. As such, a good portion of my programs are such - even the applications I enjoy on Windows. 

The programs I primarily use for writing is Neovim, which is a super version of the vi text editor. It does work well on Windows, especially in Windows Terminal. I do have a few plugins - primarily a few distraction free plugins and org.vim, which I will be touching on below.

## Organization

Like many starting points, it's always good to be organized. As such, I use org-mode, an organization format made with use for the Emacs editor, but can be used with almost any editor. In fact, Visual Studio Code has it's own org-mode plugin. As for me, I use org.vim, which provides the organizational layout of org-mode to write down the outline of my stories or even journal posts, like this one.

## Prototyping

Once I have everything organized, I then go to use Markdown to get basic markup taken care of. Markdown itself is a "What You See Is What You Mean" layout for HTML, but can be easily parsed into any other sort of document format, especially with a converter like Pandoc. Passing the markdown into pandoc with a proper output file gives me a file I can then further refactor.

## Refactoring

I take the output from Pandoc, which is a .tex file, and put into TeXworks. A .tex file is a special text preprocessor file with macros to properly typeset text. The TeX format was written by mathematician Donald Knuth back in the 70s and is still maintained today by both him and people who have made their own versions, like XeLaTeX, which is the version I use, due to the fancy fontspec package, which allows me to define my own fonts for use using TrueType formats. (I love using Garamond as my serifed font. Thank Apple for that.) 

In any case, I take this .tex file and put it into TeXworks, which allows me to preview the document and make changes to make it look right.

## Publish

Once I'm happy with the way it looks, I take the compiled preview and make it my final version. If I'm wanting an epub version of the document, I run one off with Pandoc, as it has native epub compilation. 

## End

It is a lot of work, I'll give you that, but in this case, the end really does justify the means. I'm left with a beautiful PDF document and a file I can use on an e-reader of my choice.

