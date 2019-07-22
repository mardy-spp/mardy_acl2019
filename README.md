# Who Sides With Whom? Towards Computational Construction of Discourse Networks for Political Debates

## Introduction

Understanding the structures of political debates (which actors make
  what claims) is essential for understanding democratic political
  decision-making. The vision of computational construction of such
  discourse networks from newspaper reports brings together
  political science and natural language processing.

## Dataset

423 fully annotated articles from the 2015 Tageszeitung (TAZ). 179
articles contain at least one claim. In total, 982 Claims in 764
different text passages have been annotated. This includes additional
information such as actor attributes (name, party membership, etc.),
date and position.

## Files

* codebook.pdf      : used codebook for the annotations
* train/xxxxxx.JSON : used documents for training/development
* test/xxxxxxx.JSON : used docuemnts for evaluation

## Document format

Each document is encoded as JSON file.

Following attributes are used:

* text :     String : contains complete article text (for the public version the text is scrambled for copyright reasons)
* entities:
 * begin:    character offset
 * end:      character offset
 * category: {LOC,ORG,PER}
* sentences
 * begin :
 * end :
* tokens 
 * begin :
 * end :
 * pos :

## Paper

