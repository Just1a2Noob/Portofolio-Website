---
title: 'Can Linear Regression Compete with SVM? Predicting Term Deposit Signups with Bank Data'
date: 2025-04-08T07:23:37+07:00
draft: false
hidden: false
externalURL: false
showDate: true
showModDate: true
showReadingTime: true
showTags: true
showPagination: true
invertPagination: true
showToC: true
openToC: false
showComments: false
showHeadingAnchors: true
---

This project is created with the intention of fulfiling my curiosity. Some of the questions that I hope that I can answer by doing this project is:

1. What *type* of person is interested in subscribing to a term deposit?
2. With the assumption of using just calls to tell them about term deposit, is the action of just calling enough to persuade them? If it is enough what is the minimum time needed to know we have somewhat persuaded the person?
3. Between Linear Regression and Support Machine Vector, which one is better?

The dataset that I am gona use is from a Portuguese banking institution marketing campaign. The goal of this dataset is to classify if the client will subscribe a term deposit. The original format of this file is `.arff` format which is suitable for machine learning and easier for machines to read.

To keep things simple I'm going to use only Linear Regression and Support Machine Vector, another reason why I'm using only these models is to learn the workings of both models. At the end I'm going to compare its accuracy, to determine which is better. The results of this comparison is quite surprising.

## Cleaning Data

Take a quick look at the data it's header are named using variables names, `V1, V2,...` because of this I first changed its headers to its associated description.

After that I changed the `last_contact_day` and `last_contact_month` to become one column calling it `last_contact_date`. The reason for this change is because I found it a bit weird as to why it isn't combined to a single day.
