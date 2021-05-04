# QRev-annotations

This data set contains annotated Serbian and Croatian MT outputs of English user reviews.

The source English text is compiled from the two publicly available data sets containing user reviews: 

IMDb movie reviews http://ai.stanford.edu/~amaas/data/sentiment

Amazon product reviews https://jmcauley.ucsd.edu/data/amazon/


150 reviews were selected (122 Amazon reviews and 28 IMDb reviews) containing 1170 segments and 16807 untokenised words. 
They were translated into Croatian and into Serbian by five MT systems: 
three online systems (Amazon, Bing, Google) and two in-house systems (DCU-gen and DCU-rev) trained on publicly available data.

In total, 1500 review translations were created (150 reviews translated by five MT systems into two target languages, 150*5*2). However, not all translated reviews were annotated, only a subset consisting of 452 translated reviews. 

These selected MT outputs were first given to human evaluators which highlighted all translation errors.

The evaluators were asked to annotate comprehension (comprehensibility, readability) errors (without access to the original source text), and afterwards to annotate adequacy (accuracy, fidelity) errors (by comparing the translation to the original source text). For each criterion, the evaluators were asked to distingush between major and minor errors. 
Each translation output was annotated by at least two evaluators.  In total, 15 evaluators participated in the annotation. 

When the highlighting errors was finished, one evaluator analysed the annotations and identified types and causes of marked issues. 


The evaluation had been performed in three rounds, therefore there are three folders: 

-- "first-round":  first preliminary round covering a short text (8 reviews) translated by Amazon and Google

-- "second-round": covering the remaining source text (142 reviews) translated by Amazon, Bing and Google

-- "third round":  covering a part of the source text (87 reviews) translated by the two in-house systems


The names of the files in each of these three folders are in the following format:

ROUND_SOURCE-TARGET_MT-SYSTEM_CRITERION-issue-types_EVALUATOR.txt


The format of the annotations is:

word|issue-type|highlight

An example: 

Philip|NE+NOUN_PHRASE|Major Glass|NE+NOUN_PHRASE|Major soundtrack|UNTRANSLATED+NOUN_PHRASE|Major odlično|None|None komplikuje|MISTRANSLATION+SOURCE_ERROR|Major film.|None|None


There are two more folders: 

-- "src+hyp+ref": contains all MT outputs (not only annoated) together with the source text and the reference translations into two target languages. 

-- "initial-analysis" contains results of initial analysis of relation between  comprehensibility and adequacy errors published at CoNLL 2020


The entire data set is publicly available for use under Creative Commons CC-BY. 
If you use any part of this data set, please cite the COLING paper (2020) which introduces it: 

@inproceedings{evaluation20,
Title = {Informative Manual Evaluation of Machine Translation Output},
Author = {Maja Popovi\'{c}},
BookTitle = {Proceedings of the 28th International Conference on Computational Linguistics(COLING  2020)},
year = {2020},
month = {December},
address = {Online},
}

