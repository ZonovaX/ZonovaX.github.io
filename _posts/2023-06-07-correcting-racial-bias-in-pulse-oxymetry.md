---
title: Correcting Racial Bias in Measurement of Blood Oxygen Saturation with Gradient-Boosted Forrests
author: Saad Khalid
category: machine learning
layout: post
---

<figure>
  <img src="https://i0.wp.com/www.michigandaily.com/wp-content/uploads/2021/11/madison-grosvenor-bias-oxygen-news.jpeg?resize=1536%2C1024&ssl=1" width = "350" height = "350"/>
  <figcaption>
  Source: <a href = "https://www.michigandaily.com/news/u-m-research-confirms-racial-bias-in-popular-blood-oxygen-reading-technology/">MichiganDaily.com </a>
  </figcaption>
</figure>

<p style="text-align: center;">
<strong>1st Place project out of 33 for the Erdos Institute Machine Learning Bootcamp, 2023.</strong> <br />
Team: Saad Khalid, Brooks Miner, Jaychandran Padayasi, Rohan Myers, and Woojeong Kim
</p>
<br />
Fingertip pulse oximeters are the current standard for estimating blood oxygen saturation without a blood draw, both at
home and in healthcare settings. However, pulse oximeters tend to overestimate oxygen saturation, often resulting in
‘hidden hypoxemia’: a patient has hypoxemia (dangerously low blood oxygen saturation), but the pulse oximeter returns
a healthy oxygen value. Unfortunately, oximeter overestimation of oxygen saturation is exacerbated for patients with
darker skin tones due to the interaction of skin pigment with the light-based oximeter technology. This results in Black
patients experiencing hidden hypoxemia at almost twice the rate of white patients. <br />
<br />
By combining pulse oximeter readings (SpO2) with additional patient data (such as vital signs and demographic
characteristics), we develop improved methods for estimating arterial blood oxygen saturation (SaO2) and identifying
Hidden Hypoxemia (HH). The predictions of our machine-learning models are more accurate than pulse-oximeter
readings alone, with estimates that are 30% closer to the actual blood oxygenation for patients with hypoxemia than the current medical standard of only using pulse oximetry measures. Our models also remove the systematic racial inequity inherent in the current accepted medical practice of using
oximeter readings alone. <br />
<br />
For classifying patients with hidden hypoxemia, we used an ensemble of gradient-boosted forrest classifiers. For correcting the mapping from SpO2 to SaO2, we used a gradient-boosted regression model. <br />
<br />
[See our video presentation and codebase!](https://www.erdosinstitute.org/certificates/spring-2023/data-science-boot-camp/saad-khalid) <br />
[Access a webapp showcasing a minimal feature version of the model!](https://huggingface.co/spaces/zonova/pulse_ox)