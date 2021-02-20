# Session 1.3 - Neural Style Transfer (02/09/21)

### February - Computer Vision 

---

## Preface

Good artists imitate, great artists steal, and legendary artists use a neural network to steal for them. Neural Style Transfer is a technique for applying any conceivable style to images. In this way, I could use Pablo Picasso's **Guitar Man** as a style reference, then apply the style from that painting to literally any painting I wish!

How does all of this work? It's quite intuitive. First, we define a **content** image (the image we wish to apply style to), after which we define a **style** image, whih is used to provide the aforementied style to the output image. In this scheme, a pre-trained convolutional neural network is used to extract meaningful features from both of the input images, which are used to define a loss between the generated output image and each of the style and content images. In other words, the network generates the pixels values for the output image from a blank canvas, then iteratively refines those pixel values to make the **content** more similar to the **content** image, while making the **style** of the output closer to that of the **style** image.

As you can see, Neural Style Transfer does not actually involve the training of any neural networks whatsoever! We simply modify our output over and over again to make it iteratively 'better'.

This process produces downright astonishing results. Check out the notebook below to see Neural Style Transfer in action!


## Notebook and Data

- Feb. 16, 2020 Meeting
    - Notebook: [**Neural Style Transfer | Keras**](https://www.kaggle.com/stephengregory/ai-club-nst)
    - Author: [**Stephen Gregory / TensorFlow**](https://research.google/)
    - Dataset: [**Proprietary NST Dataset**](https://www.kaggle.com/stephengregory/nst-images)

- Post-Meeting
    - Notebook: [**Neural Style Transfer | Keras**](https://www.tensorflow.org/tutorials/generative/style_transfer)
    - Author: [**Google Research / TensorFlow**](https://research.google/)
    - Dataset: [**BYOD (Bring your own Dataset)**]


## Resources
- **Neural Style Transfer:**
    - TensorFlow - [*Neural Style Transfer: Creating Art with Deep Learning*](https://medium.com/tensorflow/neural-style-transfer-creating-art-with-deep-learning-using-tf-keras-and-eager-execution-7d541ac31398)
    - [Neural Style Transfer - Wikipedia](https://en.wikipedia.org/wiki/Neural_Style_Transfer)
    - [Pytorch - Neural Style Transfer using PyTorch](https://pytorch.org/tutorials/advanced/neural_style_tutorial.html)
    - Videos:
        - [Andrew Ng Tutorial Series](https://youtube.com/playlist?list=PLO3wjWsJ4jjzv8-6SsVyU2cPB8GgUIb5o)
        - [Two Minute Papers: Universal Neural Style Transfer](https://www.youtube.com/watch?v=v1oWke0Qf1E&t=169s)
        - [Two Minute Papers: 3D Style Transfer for Videos is Now Possible!](https://www.youtube.com/watch?v=fcnjHmBcLNQ)
        - [Two Minute Papers: AI-Based Style Transfer For Video…Now in Real Time!](https://www.youtube.com/watch?v=UiEaWkf3r9A&t=206s)
- **Neural Style Transfer Papers**:
    - [A Neural Algorithm of Artistic Style](https://arxiv.org/pdf/1508.06576.pdf)
    - [Universal Style Transfer via Feature Transforms](https://arxiv.org/abs/1705.08086)
    - [Exploring the structure of a real-time, arbitrary neural artistic stylization network](https://arxiv.org/abs/1705.06830)
