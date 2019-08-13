# Introduction to cross-lingual word-embeddings at [Wikimania 2019](https://meta.wikimedia.org/wiki/Wikimania_2019)


[Word-embeddings](https://en.wikipedia.org/wiki/Word_embedding) allows machines to measure the semantic distance between a pair of words or sentences. This is done by converting each string (words or sentences) in vectors, allowing to perform mathematical operations with those strings. For example, it is possible to measure the distance between //cat// and //dog//, that might be smaller (so, they are both animals) than the distance between //cat// and //car//. 

Recently, researchers have been working in make those embeddings cross-lingual, allowing to measure the distance between strings in different languages. Therefore, translations such as //cat// [en] and //gato// [es], should very similar (ideally identical) in the vector space. 

In the [research team](https://research.wikimedia.org/) we have been using those cross-lingual embeddings to create [section alignments](https://meta.wikimedia.org/wiki/Research:Expanding_Wikipedia_articles_across_languages/Inter_language_approach#Section_Alignment) across different projects, or to align [template parameters](https://github.com/digitalTranshumant/templatesAlignment). 

The session will be organized as follows:

**First Part: Understanding and playing with cross-lingual word-embeddings** [40 mins]
* What is a word-embedding
* How to use [FastText](https://en.wikipedia.org/wiki/FastText) in Python.
* How to align models in different languages. 

**Second Part: Use cases on section alignment and recommendation ** [20 mins]
* How to query the [section alignment](https://meta.wikimedia.org/wiki/Research:Expanding_Wikipedia_articles_across_languages/Inter_language_approach#Section_Alignment) API.
* How to query the [section recommendation](https://meta.wikimedia.org/wiki/Research:Expanding_Wikipedia_articles_across_languages/Inter_language_approach#Section_Recommendation) API.

If you are just interested in using the APIs you are welcome to come just to the second part of session.

**Materials and recommendations:**

If you want to do hands-on work, and try your own alignments you will need to install some packages and download some data in advance:

* You will need a machine with at least 16GB of RAM.
* Install [Python 3 ](https://www.python.org/download/releases/3.0/) .
* Install [FastText for Python ](https://fasttext.cc/docs/en/support.html)
* Download the [models](https://fasttext.cc/docs/en/pretrained-vectors.html) (bin+vec) in [English](https://dl.fbaipublicfiles.com/fasttext/vectors-wiki/wiki.en.zip) and [Spanish](https://dl.fbaipublicfiles.com/fasttext/vectors-wiki/wiki.es.zip(. You could also download any pair of languages contained in this list:  ["es", "en", "fr", "ar", "ru", "uk", "pt", "vi", "zh", "ru", "he", "it", "ta", "id", "fa", "ca"]
* Clone this repository.

If you want to know more about word-embeddings alignments check [this repository](https://github.com/Babylonpartners/fastText_multilingual).

