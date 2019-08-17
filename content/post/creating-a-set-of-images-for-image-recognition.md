---
title: "Creating a set of images for image recognition"
date: "2019-08-11"
tags: ["computer_vision","Jeff_Blackadar","image_recognition","training"]
---

_crossposted from [Jeff's blog](http://jeffblackadar.ca/uncategorized/creating-a-set-of-images-for-image-recognition/). Jeff is an MA History and Data Science student [@CarletonU](http://carleton.ca/history)._

![iPhone camera gantry to take photos in focus at 3x magnification](http://jeffblackadar.ca/wp-content/uploads/2019/08/phone_photo_gantry_med-1.jpg)

I would like to train an image recognition model with my own images to see how well it works. Here I want to use the obverse of coins to make a model to recognize the portraits of Elizabeth II (younger), Elizabeth II (more mature), George VI and Abraham Lincoln.

Initially I used 5 cent coins but I found they reflected too much light to take a good photograph so I switched to 1 cent coins. I also started with a camera on a Microsoft Surface Pro computer, taking pictures of 9 coins at a time in order to try to be efficient, but I did not get the higher image quality I believe I need.

![Microsoft Surface Pro camera taking pictures using a Python program in Google Colab](http://jeffblackadar.ca/wp-content/uploads/2019/08/surface_pro_gantry.jpg)

![Photograph taken using the Surface Pro camera](http://jeffblackadar.ca/wp-content/uploads/2019/08/Elizabeth-II-young-2019-08-10-15_43_51.650337.jpg)

![Photo taken with iPhone: 3x magnification, square layout, flash on white paper background](http://jeffblackadar.ca/wp-content/uploads/2019/08/IMG_0282-1.jpg)

The next step is to remove the background using OpenCV in Python, crop the image to have just the coin. I don’t want to have the image recognition model recognize the portrait because her name is printed on it, so I will crop it again to have only the portrait.

I believe this type of image processing can be applied to historical artifacts photographed using a neutral background. I am concerned the coins are too worn and have too little variation in colour to make a good model but that in itself will be useful to learn if it’s the case.

My thanks to the Saskatoon Coin Club for their [excellent page](http://www.saskatooncoinclub.ca/articles/03b_1_cent_obverse.html) describing the obverse designs of Canadian one cent coins.
