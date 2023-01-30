# review_classifier
Predicting books review ratings using BERT and its variants.


# Summary
The following summarizes each notebook for Review  Classification
| Notebook                           | Description                                                                                                  | 
|:----------------------------------:|:------------------------------------------------------------------------------------------------------------:|
| [BERT for text classification](https://github.com/lilyaYAHIAOUI/review_classifier/blob/main/bert-for-text-classification.ipynb)       | A notebook which walks through fine-tuning. This notebook can be used as a template for text classification. | 
|[inference](https://github.com/lilyaYAHIAOUI/review_classifier/blob/main/inference.ipynb)                          | A notebook which walks through inference using  the ONNX Runtime accelerator.                                | 

# Dataset
This model is a fine-tuned version of bert-base-uncased on the [Goodreads Books Reviews dataset](https://www.kaggle.com/competitions/goodreads-books-reviews-290312/data). 

# Tests 
I used different models with different subsets of data. To view more details about the models check its model card.

| model         | Num epochs | Num training examples   | Num validation examples     |  model card                                                                    |
|:-------------:|:----------:|:-----------------------:|:---------------------------:|:------------------------------------------------------------------------------:|
| BERT          | 2          | 135000                  | 15000                       |[model card](https://huggingface.co/lilouuch/Goodreads_Books_Reviews_BERT_51)   |
| BERT          | 4          | 226533                  | 25171                       |[model card](https://huggingface.co/lilouuch/Goodreads_Books_Reviews_BERT_50)   |
|Roberta        | 4          | 161735                  | 17971                       |[model card](https://huggingface.co/lilouuch/Goodreads_Books_Reviews_Roberta_50)|
|distilbert     | 4          | 312935                  | 34771                       |[model card](https://huggingface.co/lilouuch/Goodreads_Books_Reviews_distilbert)|
|ALBERT         | 1          | 470097                  | 52233                       |[model card](https://huggingface.co/lilouuch/Goodreads_Books_Reviews_ALBERT)    |






### Framework versions

- Transformers 4.20.1
- Pytorch 1.11.0
- Datasets 2.1.0
- Tokenizers 0.12.1
