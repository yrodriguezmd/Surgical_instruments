# Surgical_instruments
Repo for images, annotations, notebooks and models for detecting surgical instruments.


## Objective:

Develop an application that can reliably locate and identify surgical instruments in an image.


## Workflow:

![Screen Shot 2021-10-14 at 12 16 54 PM](https://user-images.githubusercontent.com/71532604/137381676-fb69398c-05a0-476c-b9be-c052e6680043.png)

![Screen Shot 2021-10-14 at 12 17 12 PM](https://user-images.githubusercontent.com/71532604/137381699-04d04329-5d6b-4e76-bb29-7d670281390b.png)

![Screen Shot 2021-10-14 at 12 17 25 PM](https://user-images.githubusercontent.com/71532604/137381706-294c5d14-8d60-49e0-b3c2-9f1bfd2c6964.png)




[Surg_object_det_2021_10_14.pdf](https://github.com/yrodriguezmd/Surgical_instruments/files/7348795/Surg_object_det_2021_10_14.pdf)


## Summary of Results:

A series of experiments including both supervised and unsupervised learning techniques showed that fine-tuning a VFNet model with a ResNet50_fpn_mstrain_2x backbone resulted in the best level of detection, with a mAP of 82.6, validation set loss of 0.94 and good performance on the held-out test set.

Self-training using teacher- and student-models did not perform as well as conventional supervised learning.

## Deployment:

https://huggingface.co/spaces/yrodriguezmd/Surgical_instruments_app

## Reports:

https://wandb.ai/maria_rodriguez/Transfer_learning_vf/reports/Transfer-Learning-Serial-versus-One-time-Training--VmlldzoxMjczNDMz

https://wandb.ai/maria_rodriguez/Surgical_instruments_models_/reports/Choosing-a-Model-for-Detecting-Surgical-Instruments--VmlldzoxMjI4NjQ0

## Future Work:

Further improvement is needed in the detection of overlapping instruments/ dense distribution, as well as small objects (surgical needle).
