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
   * begin : character offset
   * end : character offset
* tokens 
   * begin : character offset
   * end : character offset
   * pos : Part-Of-Speech Tag
* claims
   * 
   

## Docuemnt example
```json
{
  "entities": [
    {
      "end": 3,
      "category": "I-ORG",
      "begin": 0
    },
    {
      ...
    },
    {
      "end": 535,
      "category": "I-ORG",
      "begin": 532
    }
  ],
  "sentences": [
    {
      "end": 16,
      "begin": 0
    },
    {
      ...
    },
    {
      "end": 551,
      "begin": 540
    }
  ],
  "claims": [
    {
      "quote": "Sie müssten mit der vollen Härte von Polizei und Verfassungsschutz verfolgt werden.",
      "cdate": "20151024",
      "actorvalues": [
        "30",
        "per_Yasmin Fahimi",
        "per_Generalsekretärin",
        "org_SPD"
      ],
      "claims": [
        "800",
        "811"
      ],
      "end": 444,
      "begin": 361,
      "cpos": "1"
    }
  ],
  "tokens": [
    {
      "pos": "NE",
      "end": 3,
      "begin": 0
    },
    {
      "pos": "NN",
      "end": 551,
      "begin": 540
    }
  ],
  "text": "MZM zzdgo Basvqv\n\n\nKjqirt qhlxxzg wjk \"Vvtuffkamdvvbjm\"\n\n\n\nEqdusmfv\n\n | Frj JCE helpe cpy Jxilco-Uiqlbcts pgnywuhbhhetrxubt xtx tgk gqgzoxzvll Xjpejrxldcmnrjfjlwvx. Bpzxfy ekkg qlsa dkz Infikqljscg bvhzadngy slizuhzcf Toeehklmh, patpf nmq ZIE-Feeyqvutdmyzcysry Vjnbbd Gwpnao fa Cgefilv dn Mzqedcda. Ynyg fqgdc kewo Qsfqvlhz  \"Tnmuvkzjegrm ywp Cwxvvrneaxkscu\" . Jck fndrhzv lxm akp cxixbs Rniph wjo Ypilpjd yyz Zlaflczzpbhfgimwp ahmpfklm vkdkwd. Qx Nzunbhqwxso cgim  vl dx Evtbzly pept Fklbiwlrn  bq Jzy gvk Vndrpwdycczjblatotpxxz. (yly)\n\n\n\nTantavaszyl\n\n"
}
```

## Paper

