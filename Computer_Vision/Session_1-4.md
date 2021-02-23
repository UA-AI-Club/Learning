# Session 1.4 - Real-Time Object Detection (02/23/21)

### February - Computer Vision 

---

## What is Object Detection?

Object Detection is our final major topic in Computer Vision, and it will combine what we've already learned about image classification and a new algorithmic component called **object localization**. These technologies allow neural networks to classify multiple objects in an image and label them with a coordinate bounding box, giving networks the ability to identify objects in unique context. This may seem simpler than a problem like sematic segmentation, but most computer vision applications today like autonomous vehicles and facial recognition are heavily dependent on this set of techniques. If this peaks your interest, go to [Andrew Ng's series on Coursera](https://www.coursera.org/lecture/convolutional-neural-networks/object-localization-nEeJM) for a more comprehensive understanding. 
   

## Object Localization

How does a computer find the location of objects in an image? Where do we tell our model to look? The model can't simply evaluate every possible location, since the possible combinations of horizontal/vertical position, width, and height are practically infinite. We need to quickly evaluate a small number of possible 'boxes' where the object is most likely to appear without brute-force. 
    
Back in the spring of 2016, the University of Washington colaborated with Facebook's AI Research team to present the YOLO object detection system to enable accurate reigion proposals in real time. This algorithm creates a grid of cells over an input image, each of which are evaluated on their probability of containing the **center point** of an object, rather than evaluating if the entire object is contained in the cell (as a classification model might). For each cell, the algorithm generates a few candidate bounding boxes for the object it may be centered over, and selects whichever polygon is most likely to contain our target image. 

## Combining Components

YOLO identifies these obejcts really fast, and can simultainously provide the reigons in which objects appear with the classes they represent at up to 140 FPS (depending on the architecture). 

There have been a number of iterations on the YOLO algorithm, but today we're focusing on how we can apply the latest (and somewhat controversial) YOLOv5 to almost any dataset. 


This concept is a big jump! These descriptions may appear vague (they are), but this is because the underlying math could easily take up an entire month of lessons. Note that there are a number of algorithms to approach object detection, and we've only touched the tip of an iceberg. 

### Interesting Notes:
The original creator of YOLO **Joseph Redmon** halted his CV research due to ethical concerns about the military impact of the YOLO algorithm. [Read about the controversy here](https://syncedreview.com/2020/02/24/yolo-creator-says-he-stopped-cv-research-due-to-ethical-concerns/). 

--- 

## Notebook and Data

- Meeting Demonstration:
    - **Overview Video**: [Joseph Redmon (from DarkNet) on TED](https://www.youtube.com/watch?v=Cgxsv1riJhI)
    - **Model**: [YOLOv5 - Github: ultralytics/yolov5](https://github.com/ultralytics/yolov5)
    - **Author**: [Ultralytics](https://www.ultralytics.com/)
    - **Dataset**: Trained on [Common Objects in Context](https://cocodataset.org/#home)

- Post-Meeting Practice: 
    - **Notebook**: [YOLOv3 Object Detection in Tensorflow](https://www.kaggle.com/aruchomu/yolo-v3-object-detection-in-tensorflow)
    - **Author**: ['heartkilla' - Very Impressive Profile](https://www.kaggle.com/aruchomu)
    - **Dataset**: [Data for YOLOv3 Kernel](https://www.kaggle.com/aruchomu/data-for-yolo-v3-kernel)


## Resources
- **Object Detection:**
    - Data:
        - [Common Objects in Context Benchmarks](https://paperswithcode.com/sota/object-detection-on-coco)
    - Articles:
        - [Jason Brownlee - Gentle Introduction to Object Recognition](https://machinelearningmastery.com/object-recognition-with-deep-learning/)
    - Videos:
        - [TED Talk on Object Detection](https://www.youtube.com/watch?v=Cgxsv1riJhI)
        - [Tensorflow Implementation](https://www.youtube.com/watch?v=4eIBisqx9_g) 
        - [YOLOv4 Object Detection Paper Breakdown](https://www.youtube.com/watch?v=_JzOFWx1vZg)
    - Courses:
        - [Andrew Ng - Object Detection Coursera Series](https://www.coursera.org/lecture/convolutional-neural-networks/object-localization-nEeJM)
- **Object Detection Papers**:
    - [You Only Look Once: Unified, Real-Time Object Detection](https://arxiv.org/pdf/1506.02640.pdf)
    - [**YOLOv3**: An Incremental Improvement](https://arxiv.org/abs/1804.02767)
    - [**R-CNN**: Rich feature hierarchies for accurate object detection and semantic segmentation](https://arxiv.org/pdf/1311.2524.pdf)
    - **Latest Data Augmentation Methods**: [Simple Copy-Paste is a Strong Data Augmentation Method for Instance Segmentation](https://paperswithcode.com/paper/simple-copy-paste-is-a-strong-data)