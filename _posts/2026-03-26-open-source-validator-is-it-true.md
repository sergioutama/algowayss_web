---
layout: post
title: "Open Source XBRL Validator, Can We Use It?"
date: 2026-03-26
category: Blog
description: "Practical findings on using the open-source Arelle XBRL validator with large instance documents by splitting them into smaller parts."
excerpt: "Good evening good people. Today i wanna share about open source validator for XBRL. We called it Aril (Kidding, :P). I mean arelle. You can download it from here."
original_url: "https://geexbrl.wordpress.com/2014/05/19/open-source-validator-is-it-true/"
original_date: 2014-05-19
---

*Originally published on May 19, 2014 at geexbrl.wordpress.com.*

Good evening good people. Today i wanna share about open source validator for XBRL. We called it Aril (Kidding, :P). I mean arelle. You can download it from [here](http://arelle.org/ "Arelle website").

I assume that you have installed arelle on your machine. The real problem with this tools is validating instance document with size over than 2 MB. In this case, arelle looks like stuck with validation process. So, our boss, Mr. Yudi bring idea to split instance document with maximum size 2 MB. In POC (Proof of Concept) of this idea, we use HP EliteBook 8560w with intel i7, 8 GB of Ram under windows server 2008 R2.

We are using instance document which size is 38.2 MB. First, we split that to 2 MB, so that we have 16 instance documents plus 1 instance document as aggregate from the other. After that, you can validate 16 instance document as usual, and also validate the aggregate of instance documents (Using for make sure instance is passed every interform validations). Check log error message validation, make sure that the log from 16 instance documents just have error on interform validations and the aggregate instance doesn’t has any errors.

-Gustaf Prameswara
