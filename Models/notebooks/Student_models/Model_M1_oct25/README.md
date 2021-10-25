Model_M1_oct25

When modelling using 60+ labelled data + 5K+ pseudolabels proved unpromising, more labelled data was added.

A new Teacher model Model_M_oct25 was trained using VFnet/resnet50, with 900+ labelled data, reaching a mAP of 0.6.

Pseudolabels for Set_U was generated using Model_M.

The Student model Model_M1_oct25 was trained using the Teacher model weights Model_M, using both labelled and pseudolabelled data (n= 6K+).  The mAP was in the 40's, and the valid loss was creeping up.

Next step:  add more labelled data.
