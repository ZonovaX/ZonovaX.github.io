---
title: Correlations in Sentiment Analysis of Twitter Users
author: Saad Khalid
category: machine learning
layout: post
---

<p style="text-align: center;">
<strong>Project for the Erdos Institute Machine Learning Bootcamp, 2021.</strong> <br />
Team: Saad Khalid, Wendson Barbosa, Karine Chubarian, Douglas Wagner
</p>
<br />
For many people, social media has become a primary method of consuming the news and interacting with others. Some fear this has furthered the division between people with opposing political views. Here, we test the hypothesis that social media platforms like Twitter provide an echo chamber of opinion for their users and lead to users drifting towards extremist views. <br />
<br />
Using the Twitter API, we first identify popular users whose tweets are very negative (we judge this by performing sentiment analysis on their tweets). Then we compiled lists of active followers of those popular users. We then compare the average sentiment of a users tweets before following the popular negative user to after following them. This allows us to see whether following "negative" users leads to an individual becoming more negative. <br />
<br />
[Github codebase](https://github.com/ZonovaX/SocialNetworkers) <br />
This code was written using an earlier version of Twitter's API. Due to the dramatic changes to Twitters API in 2023, the tweet-scraping code no longer functions. 