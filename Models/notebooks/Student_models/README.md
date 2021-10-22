Model_G_e will be used as the Teacher Model (Model_M).

Model_M will iteratively create pseudolabels from unlabelled datasets.

Pseudolabels will be merged to the labelled datasets.

The previous model (Model_M) will be trained using the merged labelled + unlabelled datasets to create Student models (e.g. Model_M1).
