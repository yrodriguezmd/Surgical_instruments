When iterative student model training proved ineffective and with challenging workflow, 

a whole-set (Set_U) approach was done.

The teacher Model_M (fine-tuned on labelled data Set_1_7) was used to generate pseudolabels for the whole unlabelled Set_U, generating 94% labelling.

The student Model_M1_oct_24 was trained from Model_M using the merged labelled and pseudolabelled data.

The mAP was poor at 20s-30s, with a non-improving valid loss.

Visualization of predictions on the test set showed poor-fair results.

Next step:  add more labelled data for training.
