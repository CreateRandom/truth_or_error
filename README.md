# Truth or Error? Towards systematic analysis of factual errors in abstractive summaries
Materials for our EMNLP 2020 workshop paper "Truth or Error? Towards systematic analysis of factual errors inabstractive summaries".

## Annotations
[The annotation file](all_annotations.jsonl) is in JSON lines format. Each line contains one summary. Each summary contains the name of the CNN/DM story file that contains the article that is summarized and the name of the system that was used. We also provide the sentences of the summary. Annotations are provided separately for each annotator, listing the annotations that each sentence received. 

## Sentence level error counts
This section provides a full breakdown of sentence-level errors for the different summarization systems. The meaning dimension is in the columns, the mapping dimension is in the rows.

### PG
|              |   None |   Ungrammatical |   Semantically implausible |   No meaning can be inferred |   Meaning changed, not entailed |   Meaning changed, contradiction |   Pragmatic meaning changed |
|:-------------------|-------:|----------------:|---------------------------:|-----------------------------:|--------------------------------:|---------------------------------:|----------------------------:|
| None               |    489 |               0 |                          0 |                            0 |                               0 |                                0 |                           0 |
| Omission           |      0 |              18 |                          3 |                            1 |                               0 |                                6 |                           1 |
| Wrong combination  |      0 |               7 |                          6 |                            2 |                               0 |                               13 |                           0 |
| Fabrication        |      0 |               2 |                          3 |                            0 |                               0 |                                1 |                           0 |
| Lack of re-writing |      0 |               0 |                          0 |                           21 |                               0 |                                5 |                           0 |
| Error in article   |      0 |               3 |                          0 |                            0 |                               0 |                                0 |                           0 |
| Other              |      0 |               0 |                          0 |                            0 |                               0 |                                0 |                           0 |

### Fast-Abs-RL
|              |   None |   Ungrammatical |   Semantically implausible |   No meaning can be inferred |   Meaning changed, not entailed |   Meaning changed, contradiction |   Pragmatic meaning changed |
|:-------------------|-------:|----------------:|---------------------------:|-----------------------------:|--------------------------------:|---------------------------------:|----------------------------:|
| None               |    748 |               0 |                          0 |                            0 |                               0 |                                0 |                           0 |
| Omission           |      0 |              69 |                         30 |                           12 |                               2 |                               45 |                          10 |
| Wrong combination  |      0 |               9 |                          3 |                            0 |                               2 |                                7 |                           0 |
| Fabrication        |      0 |               0 |                          1 |                            0 |                               2 |                                4 |                           0 |
| Lack of re-writing |      0 |               2 |                          0 |                           28 |                               0 |                                8 |                           0 |
| Error in article   |      0 |               2 |                          1 |                            0 |                               0 |                                0 |                           0 |
| Other              |      0 |               0 |                          0 |                            0 |                               0 |                                1 |                           0 |
### Transformer-LM
|              |   None |   Ungrammatical |   Semantically implausible |   No meaning can be inferred |   Meaning changed, not entailed |   Meaning changed, contradiction |   Pragmatic meaning changed |
|:-------------------|-------:|----------------:|---------------------------:|-----------------------------:|--------------------------------:|---------------------------------:|----------------------------:|
| None               |    365 |               0 |                          0 |                            0 |                               0 |                                0 |                           0 |
| Omission           |      0 |               2 |                          4 |                            2 |                               2 |                                1 |                           0 |
| Wrong combination  |      0 |               2 |                          5 |                            0 |                               7 |                               21 |                           0 |
| Fabrication        |      0 |               1 |                          3 |                            0 |                               7 |                                8 |                           0 |
| Lack of re-writing |      0 |               2 |                          0 |                           16 |                               0 |                                5 |                           0 |
| Error in article   |      0 |               1 |                          0 |                            0 |                               0 |                                0 |                           0 |
| Other              |      0 |               0 |                          0 |                            0 |                               0 |                                0 |                           0 |
### BertSum
|              |   None |   Ungrammatical |   Semantically implausible |   No meaning can be inferred |   Meaning changed, not entailed |   Meaning changed, contradiction |   Pragmatic meaning changed |
|:-------------------|-------:|----------------:|---------------------------:|-----------------------------:|--------------------------------:|---------------------------------:|----------------------------:|
| None               |    567 |               0 |                          0 |                            0 |                               0 |                                0 |                           0 |
| Omission           |      0 |               2 |                          1 |                            2 |                               0 |                                6 |                           2 |
| Wrong combination  |      0 |               2 |                          5 |                            2 |                               2 |                               19 |                           0 |
| Fabrication        |      0 |               2 |                          4 |                            0 |                               9 |                                6 |                           0 |
| Lack of re-writing |      0 |               1 |                          0 |                           21 |                               1 |                                8 |                           0 |
| Error in article   |      0 |               3 |                          0 |                            0 |                               0 |                                0 |                           0 |
| Other              |      0 |               0 |                          0 |                            0 |                               0 |                                0 |                           0 |

## Test set output
In our paper, we compare four summarization systems. We used the test set output the original authors have provided. This section contains the links to the original output we used.

| Approach       | Link                                                               |
|----------------|--------------------------------------------------------------------|
| PG             | https://drive.google.com/file/d/0B7pQmm-OfDv7MEtMVU5sOHc5LTg/      |
| Fast-Abs-RL    | https://drive.google.com/file/d/1m1RIc9plJD2g2fhXUvwHLRtAhTVgYFKS/ |
| Transformer-LM | https://drive.google.com/file/d/1Yu_dNiQXRScfUXVMokDXM-VXvYOQLON1/ |
| BertSum        | https://drive.google.com/file/d/1kYA384UEAQkvmZ-yWZAfxw7htCbCwFzC/ |
