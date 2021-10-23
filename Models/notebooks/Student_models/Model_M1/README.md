Model_M1 was developed by fine-tuning Model_M with the merged datasets of Set_S labelled data and Set_U1 pseudolabelled data.

Training resulted in low mAP at 30s-40s, with moderately high valid loss, and decreasing training loss.

Inference for Set_U2 resulted 66% pseudolabelling, with poor classification.

Expect that training and inference will improve with more data trained.

Note: unable to merged retained data due to discontinuity of the workflow.  

Considering gathering the unlabelled images -- to either annotate manually or to pass again in an inference step in a later model.
