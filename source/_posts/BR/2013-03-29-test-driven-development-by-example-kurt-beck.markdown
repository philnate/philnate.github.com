---
layout: post
title: "Test Driven Development. By Example (Kurt Beck)"
date: 2013-03-29 23:34
comments: true
categories: ["Book review"]
tags: ["TDD"]
---
##Introduction
Lately I started to learn _Test Driven Development (TDD)_ as I was bugged, by recent flaws. I heard that Kent Beck (re)invented TDD so it obvious to grap a book written by him if available.  
After a short search I found _Test Driven Development. By Example_, which gives a really good introduction into TDD.

##The Book -- Overview
The Book is three parted, each part containing several chapters.

* Part I gives an introduction into TDD by writing some Money class
* Part II ?????
* Part III

###Part I

###Part II

###Part III

###Conclusion

##Personal experience
Practicing TDD really gives a good feeling and improves somewhat the confidence about the code you've written. As it's required that you can test everything you don't end up with some black-box where some parts can't be tested (obviously). I just have seen it too often lately that some bugs where discovered, but the old non TDD code blocked writing a regression test for it. Leaving a really bad feeling that it will eventually break again without noticing it. So getting a book about refactoring legacy code to the good is some of the follow up readings.  
As TDD is quite new too me, I've catched myself more than once writing the implementation before the actual Tests. But I'll guess that's just normal in this stage.  
What I wonder is how you do some quick testing like, _does this 3rd party library fulfill my requirements?_ I encounter this situation quite often, where I write code which is soon dropped as the used library doesn't fit my needs. In these situations I don't want to be loaded with writing tests for code I'm most likely dropping soon after again. Once I've found the solution I'm going to use I'll never can write this code TDD.  
Most likely this shows me that the taken step, was just too big to be solved cleanly in a TDD manner.
