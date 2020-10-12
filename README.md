# Truth or Error? Towards systematic analysis of factual errors in abstractive summaries
Materials for our EMNLP 2020 workshop paper "Truth or Error? Towards systematic analysis of factual errors inabstractive summaries".

## Annotations
[The annotation file](all_annotations.jsonl) is in JSON lines format. Each line contains one summary. Each summary contains the name of the CNN/DM story file that contains the article that is summarized and the name of the system that was used. We also provide the sentences of the summary. Annotations are provided separately for each annotator, listing the annotations that each sentence received. 

## Test set output
In our paper, we compare four summarization systems. We used the test set output the original authors have provided. This section contains the links to the original output we used.

| Approach       | Link                                                               |
|----------------|--------------------------------------------------------------------|
| PG             | https://drive.google.com/file/d/0B7pQmm-OfDv7MEtMVU5sOHc5LTg/      |
| Fast-Abs-RL    | https://drive.google.com/file/d/1m1RIc9plJD2g2fhXUvwHLRtAhTVgYFKS/ |
| Transformer-LM | https://drive.google.com/file/d/1Yu_dNiQXRScfUXVMokDXM-VXvYOQLON1/ |
| BertSum        | https://drive.google.com/file/d/1kYA384UEAQkvmZ-yWZAfxw7htCbCwFzC/ |
