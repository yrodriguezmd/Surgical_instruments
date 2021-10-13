Contains the initial set of images.  

15 classes:




![Screen Shot 2021-10-13 at 4 41 35 PM](https://user-images.githubusercontent.com/71532604/137227399-ec5193b3-fc2c-4c64-983a-e7f94931f1f8.png)

10 representative images per class.

Utilize pretrained RetinaNet to produce pseudolabels from the inference.

Refine labels in annotation tool (Roboflow).

Upload refined annotations, use to fine tune RetinaNet to iteratively generate the Teacher model.
