# Arabic Singular-to-Plural Conversion

This repository contains the data files and Jupyter notebooks required to reproduce the models and results reported in our *"Neural Arabic Singular-to-Plural Conversion with a Pre-trained Character-BERT and a Fused Transformer"* paper.

This work aims at approaching the MIG task suggested by [SIGMORPHON](https://github.com/sigmorphon/2022InflectionST/blob/main/part2/README.md). We start with pre-training an Arabic Character-BERT on the MLM task, and then fusing it into a transformer encoder-decoder model.

The links provided in the notebooks are downloadable, and hence no extra coding is required to enable their running. It is necessary to run the notebooks using Google Colab, otherwise when reading the files from their paths an error will be raised, unless the paths are corrected correspondingly.
