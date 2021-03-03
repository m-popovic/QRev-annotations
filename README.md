# QRev-annotations

This data set contains annotated Serbian and Croatian MT outputs of English user reviews.

The source English text is compiled from the two publicly available data sets containing user reviews: 

IMDb movie reviews http://ai.stanford.edu/~amaas/data/sentiment

Amazon product reviews https://jmcauley.ucsd.edu/data/amazon/


In total, 150 reviews were selected (122 Amazon reviews and 28 IMDb reviews) and translated into Croatian and into Serbian by five MT systems: 

three online systems (Amazon, Bing, Google) and two in-house systems (DCU-general-domain and DCU-review-domain) 


The outputs are then given to human evaluators which highlighted all translation errors.

The evaluators were asked to annotate comprehension (comprehensibility, readability) errors (without access to the original source text), and afterwards to annotate adequacy (accuracy, fidelity) errors (by comparing the translation to the original source text). 

Each translation output was annotated by at least two evaluators. 






If you use any part of this data set, please cite the COLING paper (2020) which introduces it: 

@inproceedings{evaluation20,

Title = {Informative Manual Evaluation of Machine Translation Output},

Author = {Maja Popovi\'{c}},

BookTitle = {Proceedings of the 28th International Conference on Computational Linguistics(COLING  2020)},

year = {2020},

month = {December},

address = {Online},

}

