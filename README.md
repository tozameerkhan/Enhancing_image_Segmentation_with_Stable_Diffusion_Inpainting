# Enhancing-Image-Segmentation-with-Stable-Diffusion-Inpainting

Stable Diffusion is an impressively powerful text-to-image model released by Stability AI earlier this year. In this blog post, we’ll explore a technique for augmenting training data with Stable Diffusion in order to improve performance on an image segmentation task. This approach is especially powerful in applications where data is limited or would otherwise require tedious human labeling.

In the context of computer vision models, image segmentation refers to splitting an image into two or more components based on its contents. In contrast to “image classification”, the goal of segmentation is to not only identify what an image contains, but which parts of the image correspond to each class.

Specifically, we will be taking a look at the DeepGlobe Road Extraction Dataset, which consists of around 6,000 aerial photographs of rural roads. The task for this dataset is to separate images into two classes: “road” and “background”. The dataset also comes with training labels in the form of mask images, where roads are identified in white and background is in black.
