---
title: XLNet Large
author: John Snow Labs
name: xlnet_large_cased
date: 2020-04-28
tags: [embeddings, en, xlnet]
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description
XLNet is a new unsupervised language representation learning method based on a novel generalized permutation language modeling objective. Additionally, XLNet employs Transformer-XL as the backbone model, exhibiting excellent performance for language tasks involving long context. Overall, XLNet achieves state-of-the-art (SOTA) results on various downstream language tasks including question answering, natural language inference, sentiment analysis, and document ranking. The details are described in the paper "[​XLNet: Generalized Autoregressive Pretraining for Language Understanding](https://arxiv.org/abs/1906.08237)"

{:.btn-box}
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/xlnet_large_cased_en_2.5.0_2.4_1588074397954.zip){:.button.button-orange.button-orange-trans.arr.button-icon}

## How to use

{% include programmingLanguageSelectScalaPython.html %}

```python

embeddings = XlnetEmbeddings.pretrained("xlnet_large_cased", "en") \
      .setInputCols("sentence", "token") \
      .setOutputCol("embeddings")
```

```scala

val embeddings = XlnetEmbeddings.pretrained("xlnet_large_cased", "en")
      .setInputCols("sentence", "token")
      .setOutputCol("embeddings")
```

{:.model-param}
## Model Parameters

{:.table-model}
|---|---|
|Model Name:|xlnet_large_cased|
|Type:|embeddings|
|Compatibility:|Spark NLP 2.5.0|
|Edition:|Official|
|Spark inputs:|[sentence, token]|
|Spark outputs:|[word_embeddings]|
|Language:|[en]|
|Dimension:|1024|
|Case sensitive:|true|
|License:|Open Source|

{:.h2_title}
## Source
The model is imported from [https://github.com/zihangdai/xlnet](https://github.com/zihangdai/xlnet)