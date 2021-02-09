# Session 1.2 - Semantic Segmentation (02/09/21)

### February - Computer Vision 

---

## Preface

Semantic Segmentation uses computer vision architecture to classify individual features, or segments, in an image by assigning class labels to every pixel in the input raster image. Segmentation models frequently use the same convolutional kernels seen in the previous classification models, but in an hourglass-like architecture. The input half of the hourglass compresses (encodes) the data in our image, and the latter half mirrors its structure to extract (decode) the learned features. This has openend up a wide set of contemporary machine learning solutions ranging from autonomous vehicles, to biomedical imaging, and geospatial data analysis (see resources). The notebook we've picked for semantic segmentation works with aerial imagery for autonomous drone navigation. Please enjoy!


## Notebook and Data

- Notebook: [**Deep Learning based Semantic Segmentation | Keras**](https://www.kaggle.com/bulentsiyah/deep-learning-based-semantic-segmentation-keras)
- Author: [**Bulent Siyah**](https://www.kaggle.com/bulentsiyah)
- Dataset: [**Aerial Semantic Segmentation Drone Dataset**](https://www.kaggle.com/bulentsiyah/semantic-drone-dataset)


## Resources
- **Semantic Segmentation:**
    - [Semantic Segmentation Guide for 2021](https://nanonets.com/blog/semantic-image-segmentation-2020/)
    - TDS - George Seif's [*Semantic Segmentation with Deep Learning*](https://towardsdatascience.com/semantic-segmentation-with-deep-learning-a-guide-and-code-e52fc8958823)
    - [Image Segmentation - Wikipedia](https://en.wikipedia.org/wiki/Image_segmentation)
    - [Pytorch - Semantic Segmentation using Torchvision](https://learnopencv.com/pytorch-for-beginners-semantic-segmentation-using-torchvision/)
    - Brief Pytorch Models:
        - [UNET](https://pytorch.org/hub/mateuszbuda_brain-segmentation-pytorch_unet/)
        - [DEEPLABV3-RESNET101](https://pytorch.org/hub/pytorch_vision_deeplabv3_resnet101/)
    - Top Performance Benchmarks for Image Segmentation:
        - [Cityscapes](https://paperswithcode.com/sota/semantic-segmentation-on-cityscapes)
        - [PASCAL VOC](https://paperswithcode.com/sota/semantic-segmentation-on-pascal-voc-2012)
        - [PASCAL Context](https://paperswithcode.com/sota/semantic-segmentation-on-pascal-context)
    - [Tensorflow Tutorial on Semantic Segmentation](https://www.tensorflow.org/tutorials/images/segmentation)
    - [Papers with Code: Semantic Segmentation](https://paperswithcode.com/task/semantic-segmentation)
- **Semantic Segmentation Papers**:
    - [U-Net: Convolutional Networks for Biomedical Image Segmentation](https://paperswithcode.com/paper/u-net-convolutional-networks-for-biomedical)
    - [ResNeSt: Split-Attention Networks](https://arxiv.org/abs/2004.08955v2)
    - Google's [Rethinking Atrous Convolution for Semantic Image Segmentation](https://paperswithcode.com/paper/rethinking-atrous-convolution-for-semantic)
    - [DeepLab: Semantic Image Segmentation with Deep Convolutional Nets, Atrous Convolution, and Fully Connected CRFs](https://paperswithcode.com/paper/deeplab-semantic-image-segmentation-with-deep)
    - **Bonus**: [An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale](https://arxiv.org/abs/2010.11929)