---
title: "Computational Creativity and Archaeological Data Project - Getting Started"
date: "2019-08-09"
tags: ["computational_creativity","computer_vision","Jeff_Blackadar"]
---

_crossposted from [Jeff's blog](http://jeffblackadar.ca/uncategorized/computational-creativity-and-archaeological-data-project/). Jeff is an MA History and Data Science student [@CarletonU](http://carleton.ca/history)._

I am doing research for the Computational Creativity and Archaeological Data project. My current challenge has been to use techniques from Computer Vision to analyse images relevant to Computational Research on the Ancient Near East ([CRANE](https://crane.utoronto.ca/)) with the goal to provide additional understanding of these images. Computer Vision and machine learning could identify and classify elements in images or provide a possible reconstruction of a partial artifact using an image of it combined with a model of images of related artifacts. Here, I would like to reference Ivan Tyukin, Konstantin Sofeikov, Jeremy Levesley, Alexander N. Gorban, Penelope Allison and Nicholas J. Cooper’s work “Exploring Automated Pottery Identification [Arch-I-Scan]” in _Internet Archaeology_ 50. [https://doi.org/10.11141/ia.50.11](https://doi.org/10.11141/ia.50.11)

In order to classify images I plan to use machine learning. To do this I need a workable method, a machine learning platform and then to create a model that can be used for image recognition.

The method I plan to use is described in the books [Deep Learning with Python](https://www.manning.com/books/deep-learning-with-python)/[R](https://www.manning.com/books/deep-learning-with-r). Using the techniques from the book, I can train a model to recognize different types of images and so far I have been able to make the examples in the book work.

[Google Colab](https://colab.research.google.com/notebooks/welcome.ipynb#recent=true) is the machine learning platform I am using. I am comfortable using this given I am not using any sensitive data as per guidelines [here](https://jeffblackadar.github.io/image_work/). Colab offers a free GPU which is a requirement for the efficient processing of these models. (Training one model was going to take 2 hours without a GPU. With a GPU it took a few seconds.)

**Python vs. R**. Colab has some support for R but it did not work well enough to install what was required. I have switched to Python. This is the [notebook of my setup](https://github.com/jeffblackadar/image_work/blob/master/deep_learning_with_python_appendix_a.ipynb) of Colab.

I have made examples from _Deep Learning with Python_ work. Now I want to create my own sets of training data, train models with them and see the results. This will provide a better understanding of the limitations and pitfalls of using machine learning for image recognition.
