# Automated Text Summarization for Dialogues with Transformer Models
This thesis is dedicated to the automated summarisation of texts and dialogues and covers the
implementation of different approaches. While text summarisation is already a well-known
topic in the Natural Language Processing (NLP) domain, there are only a few approaches that
specialise in summarising dialogues between several parties in a user-friendly way (e.g. to-do
list that emerges from a meting transcript). It is shown that the classification of action
items in dialogues is technically possible with the help of RoBERTa which achieves very
good results. Another approach proposes the supervised sequence-to-sequence generation of
a summary with BART. However, the available data which is needed to train both of these
models, is not mature enough and too domain specific. If new corpora or datasets emerge
that address these shortcomings, the approaches should be revisited in future work.
In another attempt, which is based on transcripts of political debates, the individual utterances
are assigned to dialogue type categories. The longest 10% of the utterances are monologues
which are abstractly summarised using a transformer model and on average still have 25%
of their original length. The next 15% longer utterances are statements, which are also
summarised using a transformer model but contain a constant length of 5-15 tokens. The
remaining utterances are merged into discussion blocks of a parameterisable length. TF-IDF
is then used to extract the most important key words from the discussion blocks. The
extracted key words are then assigned to the individual utterances. This algorithm delivers
results that are easy to interpret and provide a high degree of relevant information. The user
is thus able to avoid 90% of the original transcript, thus saving a lot of time.

## Unsupervised_Text_Generation_Key_Word:

![alt text](https://github.com/loran-avci/dialog_summ/blob/master/Unsupervised_Text_Generation_Key_Word/img/example.png?raw=true)

Code, data (csv, txt, mp3) and Summarys (xlsx, html) to the Unsupervised Text Generation and Key Word Extraction approach.
Documentation is available in the Jupyter Notebook.
For more information see chapter 2.3 of Automated Text Summarization for Dialogues with Transformer Models.


## Supervised_Text_Generation:
Code and data to the Supervised Text Generation approach. 
No documentation for code available.
For more information see chapter 2.2 of Automated Text Summarization for Dialogues with Transformer Models.

## Action_Item_Classification:
Code and data to the Action Item Classification approach. 
No documentation for code available.
For more information see chapter 2.1 of Automated Text Summarization for Dialogues with Transformer Models.


