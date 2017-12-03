# Pos-taggers
Part-of-speech taggers for Kazakh language.
Used PoS tagger models:
- Trigrams'n'Tags(TnT) from [python's nltk package](http://www.nltk.org/_modules/nltk/tag/tnt.html).  
- [RDRPOSTagger](http://rdrpostagger.sourceforge.net/)
- [Conditional Random Fields (CRFs)](https://sklearn-crfsuite.readthedocs.io/en/latest/)

Used datasets:
- [Universal Dependencies](https://github.com/UniversalDependencies/UD_Kazakh)(UD)
- [Kazakh Language Corpora](http://kazcorpus.kz/klcweb/en/)(KLC)


# Installation
Run `conda create -n myenv --file package-list.txt`

# Calculate accuracy of RDRPOSTagger
## For KLC
Run `python Eval.py full-path-to/klc.raw_test.TAGGED full-path-to/klc.test`
## For UD
Run `python Eval.py full-path-to/kazcorpus_raw_test.TAGGED full-path-to/kazcorpus_test`

For more details see http://rdrpostagger.sourceforge.net/
