---
title: Multi‑Modal Forecasting of Precipitation using a Deep Convolutional Network
author: Saad Khalid
category: machine learning
layout: post
---

<figure>
  <img src="https://nbviewer.org/github/MIT-AI-Accelerator/eie-sevir/blob/master/examples/tutorial_img/sevir_sample.gif"/>
  <figcaption>
  Sample event in the <a href = "https://nbviewer.org/github/MIT-AI-Accelerator/eie-sevir/blob/master/examples/SEVIR_Tutorial.ipynb">SEVIR dataset</a>
  </figcaption>
</figure>

Weather forecasting involves making predictions on an incredibly high-dimensional and chaotic system. The standard physics based simulations provide the cutting edge of accuracy, but are notoriously computationally expensive, and the computational cost to increasing their accuracy scales exponentially. Utilizing the pattern recognition abilities of AI has the potential to give faster predictions which scale more efficiently, allowing for more accurate predictions that reach further into the future. Techniques developed for weather forecasting can also be applied in a wide array of other cutting edge fields, ranging from video generation to predicting trends in financial markets. <br />
<br />
I approached this as an Image-to-Image problem. I generalized a [two-stream CNN](https://arxiv.org/abs/1406.2199) to a U-Net architecture, and used OpenCV to generate the optical flow of the evolving precipitation maps. The model is then trained on over 10,000 multi-modal weather events sourced from the SEVIR database, with input consisting of 13 frames of original precipitation maps (each separated by 5 minutes) and their corresponding optical flow frames, and output being a prediction of the following 12 frames of precipitation. <br />
<br />
[Github codebase](https://github.com/ZonovaX/Weather_Forecasting_SEVIR)