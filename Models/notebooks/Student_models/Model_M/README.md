COCO-pretrained VFnet model with a resnet50_fpn_mstrain_2x backbone was fine-tuned using the labelled dataset Set_S (Set_1_7) (n=677).

This Teacher model Model_M had a mAP of 51.8 after 120 epochs of training.

Model_M was used to generate pseudolabels for the unlabelled Dataset_U1 (n=1479), 92% of which had pseudolabels after inference.


Trial of merging were done:

The pseudolabelled images were merged to Set_S/train, and

the unlabelled paths were saved as 'Set_U1_a'.
