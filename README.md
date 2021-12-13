# instance_segmentation_nuclei
---
for TA: if you want to reproduce the submission
you can download the `inference.ipynb` and run all
---
## task
2018 nuclei instance segmentation but lower training data size and larger image size(1000x1000)
## Environment
- colab GPU(Tesla P100)
## packages
- pytorch
- mmcv
- numpy
- pyyaml==5.1
- detectron2

## introduction
there are 
- 5 ipynb files

**1. Prepare_anno.ipynb**</br>
this file convert initial dataset to coco instance segmentation format.
**2. unet.ipynb**</br>
A try on using unet to do "semantic segmentation", and try to convert the output to our nuclei instance segmentation
the reason why I use it is because this homework only has "one" instance category.
But I failed to convert semantic map to instances
**3. inference.ipynb**</br>
modified from the ipynb file TA attached.
**4. experiments.ipynb**</br>
this file record all experiments about trying different backbone or different  models.
**5. main.ipynb**</br>
record the best setting , including model, backbone, model parameters setups...
## reproduce
- download `inference.ipynb` and just run it on colab.

**note** 
The model para and all py files you need to reproduce the submission are embedded in the `inference.ipynb`,</br> but if you want to check my weight para is normal,</br>please follow this [link](https://drive.google.com/file/d/1FJaP6zLHRQNvB4aOM8IfnNvI_MHIujDK/view?usp=sharing)
## reference
[1] https://github.com/facebookresearch/detectron2 </br>
[2] https://neptune.ai/blog/image-segmentation-tips-and-tricks-from-kaggle-competitions</br>
[3] PointRend: Image Segmentation as Rendering.by Alexander Kirillov.et al.</br>
[4] https://github.com/open-mmlab/mmdetection</br>
[5] https://github.com/facebookresearch/detectron2</br>
[6]https://github.com/facebookresearch/detectron2/blob/main/detectron2/config/defaults.py</br>
[7] A Survey on Instance Segmentation: State of the art, by Abdul Mueed Hafiz et al.</br>
[8] U-Net: Convolutional Networks for Biomedical Image Segmentation.by Olaf Ronneberger et al.</br>
[9]https://www.reddit.com/r/computervision/comments/bmrj4h/best_instance_segmentation_for_small_objects/ </br>




