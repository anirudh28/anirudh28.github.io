---
title: "Future Video Frame Segmentation Prediction"
excerpt: "Project to predict the segmentation mask of the 22nd frame of a video using the first 11 frames<br/><img src='/images/Future_Segmentation_Prediction.png'>"
collection: portfolio
---

In this work, we present different solutions for future segmentation prediction. Our goal is to predict the 22nd frame using the first 11 frames in synthetic videos consisting of 48 different 
objects distinguished by shape, color and texture. We employ CNN based models for motion prediction and transformer based models for segmentation mask computations. We first train SimVP to 
predict the 22nd frame from the first 11 frames and use this model to predict the 22nd frame as an intermediate result. We then train the Segformer model to predict segmentation masks of images 
and run it on the frames predicted by SimVP to get the final output. We use the Jaccard similarity index to evaluate our model. 
[Report](https://drive.google.com/file/d/1V2Es7hxqr4Xz4NaXwPqecYN1V652BbOe/view?usp=sharing) [Code](https://github.com/anirudh28/Video-Frame-Prediction)
