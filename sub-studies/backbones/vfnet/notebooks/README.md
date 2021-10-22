
![Screen Shot 2021-10-21 at 4 36 49 PM](https://user-images.githubusercontent.com/71532604/138371010-ddd9bc33-723c-40fa-a24a-6fa1b0606288.png)

#### Inference using Set_1_7 test_set (preds_saved) samples:

![Screen Shot 2021-10-21 at 4 51 41 PM](https://user-images.githubusercontent.com/71532604/138372128-0973a19a-52a6-4843-b6a7-34560f846f87.png)

#### Summary:

1.  Deeper layers and VF net produce slightly better bboxes.
2.  Classes prediction are comparable between the five backbones.
3.  Deeper nets take longer to train and gave better mAP, especially in VFnet, however, viusal inspection reveals that this is not very significant.
4.  VFnet/resnet50_fpn_mstrain_2x has the same training time as VFnet/resnet50_fpn_1x, but gives better mAP.
5.  Losses are bigger for VFnet, however, mAPs are generally higher.

#### Decision:

Use VFNet/resnet50_fpn_mstrain_2x as the structure for training the Teacher Model.
