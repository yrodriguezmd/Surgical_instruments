A Teacher model was generated using conventional supervised learning techniques.  A mAP of 82.6 was reached using VFNet/resnet50_fpn_mstrain_2x within 100 epochs of training.

Pseudolabels were generated for ~5000 unlabelled images using the Teacher model.

A Student model was fine-tuned using both labelled and pseudolabelled data.  The mAP and validation set loss was not better than that of the teacher model.  Training stopped at 40 epochs.  Dashboard: 
https://wandb.ai/maria_rodriguez/Surg_self_training

![Screen Shot 2021-11-30 at 10 59 55 AM](https://user-images.githubusercontent.com/71532604/144110639-a3cebf17-ce40-4edb-b8d9-f26b214acfc3.png)
