---
layout: post
title: "Gaussian Process (GP): A Brief Introduction"
description: "What is GP? Why is it useful?"
comments: true
---

This post aims to provide a simple introduction to Gaussian Process (GP) for regression purposes.

It's that time of the year when a major vision conference [releases the papers to the public](http://openaccess.thecvf.com/CVPR2018.py), so it's time to check how deep learning is doing in their titles.<br>
<br>
At ICCV 2017, we realized that [GANs were growing strong]({{ site.url }}/gans-et-al-growing-strong/), and before we did a set [of]({{ site.url }}/dl-lstm-gan-evolution) [posts]({{ site.url }}/deep-learning-scraping/) of [the]({{ site.url }}/deep-learning-plateau/) [deep learning]({{ site.url }}/deep-learning-takes-over-again/) [saga]({{ site.url }}/deep-learning-evolution/).<br>
<br>
Let's update the plots to CVPR 2018, as always, using the XKCD style, as described in this [blog post]({{ site.url }}/xkcd-deep-learning/), but this time putting all trends together:
<br />
<img align="middle" width="500" src="{{ site.url }}/images/deep_vs_gan_evolution.png" alt="...">
<br />
<br />

So, general deep-learning keywords are getting out of fashion (we take them for granted), but GANs are no longer such a minority (8\%!). LSTM, on the other hand, cannot keep up. Will GANs catch up with general deep learning?<br />
<br />
Are GANs the new Deep?


asdasdadsad

<br />
asdasdasdasdasd
## No rattler - no rattler
<HTML>
<HEAD> <TITLE>Activity - Insert animated GIF to HTML</TITLE> </HEAD>
<BODY>
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_1_2.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_1_3.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_1_5.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_1_6.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_1_8.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_1_9.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_1_11.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_1_12.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_1_14.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_2_3.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_2_5.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_2_6.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_2_8.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_2_9.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_2_11.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_2_12.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_2_14.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_3_5.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_3_6.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_3_8.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_3_9.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_3_11.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_3_12.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_3_14.gif" alt="...">  
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_5_6.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_5_8.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_5_9.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_5_11.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_5_12.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_5_14.gif" alt="...">    
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_6_8.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_6_9.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_6_11.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_6_12.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_6_14.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_8_9.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_8_11.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_8_12.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_8_14.gif" alt="..."> 
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_9_11.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_9_12.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_9_14.gif" alt="...">    
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_11_12.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_11_14.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_12_14.gif" alt="...">      
</BODY>
</HTML>
  
## No rattler - one rattler
<HTML>
<HEAD> <TITLE>Activity - Insert animated GIF to HTML</TITLE> </HEAD>
<BODY>
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_1_4.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_1_7.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_1_13.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_2_4.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_2_7.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_2_13.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_3_4.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_3_7.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_3_13.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_5_4.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_5_7.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_5_13.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_6_4.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_6_7.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_6_13.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_8_4.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_8_7.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_8_13.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_9_4.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_9_7.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_9_13.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_11_4.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_11_7.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_11_13.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_12_4.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_12_7.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_12_13.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_14_4.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_14_7.gif" alt="...">
  <img align="middle" width="500" src="{{ site.url }}/images/research/zts_14_13.gif" alt="...">  
</BODY>
</HTML>
    
