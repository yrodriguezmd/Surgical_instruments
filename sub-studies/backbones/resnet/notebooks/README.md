
#### Using merged dataset Set_1_7, models were fine-tuned using COCO-pretrained RetinaNet with the following backbones:

Resnet50 (Model_G_a) and 

Resnet101 (Model_G_b)

![Screen Shot 2021-10-20 at 3 19 06 PM](https://user-images.githubusercontent.com/71532604/138180424-eca84405-0934-4eae-a58d-3865f48e7124.png)


Show_results (valid_ds) samples (Model_G_b):

![Screen Shot 2021-10-20 at 3 19 46 PM](https://user-images.githubusercontent.com/71532604/138180489-3707834f-9d13-4f14-8a69-9117e0f73282.png)


Inference using Set_1_7 test_set (Model_G_b) samples:

![Screen Shot 2021-10-20 at 3 20 19 PM](https://user-images.githubusercontent.com/71532604/138180542-7d4027c0-66d0-46f6-864a-746bfde8cafe.png)


Comparison of Results:

Ground Truth  --   RetinaNet/ Resnet50 (Model_G_a) -- RetinaNet/Resnet101 (Model_G_b)

![Screen Shot 2021-10-20 at 3 34 47 PM](https://user-images.githubusercontent.com/71532604/138182429-4baadae2-165b-445c-9418-7de906e8cfb5.png)


![Screen Shot 2021-10-20 at 3 36 09 PM](https://user-images.githubusercontent.com/71532604/138182339-bf61b8c6-457b-49d1-a20b-61a8505b17b7.png)


![Screen Shot 2021-10-20 at 3 36 28 PM](https://user-images.githubusercontent.com/71532604/138182353-dceaccab-e7be-4773-bd0d-571d0c144ec8.png)

![Screen Shot 2021-10-20 at 3 36 50 PM](https://user-images.githubusercontent.com/71532604/138182364-cba2d64f-6d27-4016-816a-96f246f43f70.png)
![Screen Shot 2021-10-20 at 3 37 56 PM](https://user-images.githubusercontent.com/71532604/138182370-31839c03-2866-4357-9b83-1f5eb28091d6.png)

![Screen Shot 2021-10-20 at 3 35 25 PM](https://user-images.githubusercontent.com/71532604/138182428-f1065856-7ee7-4e01-92fd-b76c448edd1f.png)


![Screen Shot 2021-10-20 at 3 38 11 PM](https://user-images.githubusercontent.com/71532604/138182384-8bd21c66-b87e-4bb3-b8b9-dd8a5284bde0.png)

![Screen Shot 2021-10-20 at 3 35 46 PM](https://user-images.githubusercontent.com/71532604/138182427-a6d842ff-a0bc-4d6d-87e3-c0d43ca0db9c.png)




Summary of Results:

1)  Iterative model training (from Model_A_ to Model_G) had similar results with 1-stage training (Model_G_a and Model_G_b).
2)  Iterative training and pseudolabel generation offers the benefit of labelling-assistance in creating datasets.
3)  The Resnet101 backbone (Model_G_b) confers a slightly better mAP and loss values compared to a Resnet50 backbone (Model_G_a), at a price of longer train run.
4)  Resnet101 have tighter bboxes, but Resnet50 have slightly better classifications.

Interpretation:

Resnet50 is a good option for modelling surgical instruments, providing good bboxes, good classification with reasonable training time.
