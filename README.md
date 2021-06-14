# Machine-learning-for-aquatic-plastic-litter-detection-and-classification
The project is an application of computer vision-object detection. We made a model using Mask R-CNN to detect presence of plastic objects like food wrappers, plastic water bottles, food containers etc that are floating around on the surface of water bodies. We intend to us this application to clean water bodies and reduce pollution caused by plastics.

![Screen Shot 2021-06-15 at 12 59 11 AM](https://user-images.githubusercontent.com/30744863/121949129-be269780-cd75-11eb-99e9-213539b6b913.png)

Modules:

![Screen Shot 2021-06-15 at 12 58 54 AM](https://user-images.githubusercontent.com/30744863/121949143-c41c7880-cd75-11eb-84ad-cbde53eba39e.png)

Methodology:
Project uses mask R-CNN approach which can briefly consists of two stages i.e. generate proposal regions where the objects might be present followed by prediction od classes, refine bounding box and generate mask at the pixel level. These two stages are connected by backbone ResNet50. This method of generating proposal regions instead of selecting high number of regions like CNN is called selective search method.
In step 1 the input image is fed to the model where a light weight neural network called RPN is used to scan all the feature pyramid networks to extract a feature map. This is don using top-bottom pathway that generated proposal regions which may contain objects.

Labelling:

![Screen Shot 2021-06-15 at 12 58 49 AM](https://user-images.githubusercontent.com/30744863/121949196-ced70d80-cd75-11eb-854a-55df8adc658a.png)

Input:

![Screen Shot 2021-06-15 at 1 06 14 AM](https://user-images.githubusercontent.com/30744863/121949302-eca47280-cd75-11eb-9cf0-4225f3690e7e.png)

Output:

![Screen Shot 2021-06-15 at 1 06 19 AM](https://user-images.githubusercontent.com/30744863/121949319-f29a5380-cd75-11eb-961d-775de21b3dfe.png)

WebApplication for the same:

![image2](https://user-images.githubusercontent.com/30744863/121949339-fb8b2500-cd75-11eb-978d-6faaceff374c.png)

