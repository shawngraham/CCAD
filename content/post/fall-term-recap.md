---
title: "Fall 2019 Recap"
date: "2020-01-09"
tags: ["computer_vision","Jeff_Blackadar","image_recognition","training", "pompeii"]
---

I've done not a particularly good job of keeping this website up to date. But we have been busy.

In the fall, we arranged for some more data science training for Jeff, and he's been working hard on learning Keras and other packages and approaches for the various tasks we have in mind for this project. I've been reposting some of his open research notes here, but since I've fallen behind, I'll just link over to his notes [here](http://jeffblackadar.ca/).

We are still exploring how to teach the computer to imagine like an archaeologist. An archaeologist can look at a partial profile of a pot or a piece of architecture, and based on their training and experience, they'll be able to make a reasonable reconstruction of the entire piece. They're helped by the regularity of forms and so on, even though there are times when folks in the past did something that throws us a curveball. Which is to say: why can't we teach machines to make those same intuitive leaps?

In which case, we've been looking at image in-painting as one way of doing this. We take an  image that the machine hasn't seen before, and mask out areas of the image. Based on its training, the machine then tries to fill the image. Since we know what the complete image looks like, we can measure the degree of success, then tweak things and try again.

Another thing we're exploring is hallucinating whole images from scratch (that is, using generative adversarial images). What truth(s) might this approach show us?

Going even further out on the limb, we want to use these adversarial images as fodder for photogrammetry. Can we also do something akin to 2d image inpainting with 3d models?

The problem is one of data. While this work that Jeff and I are doing is a subproject of the larger CRANE project, we don't have any near eastern materials to work with. I have no archaeological archives I've created that I can readily tap. It's been a while since I was in the field. So we looked at a variety of online repositories, for pottery, for all sorts of things. [Open Context](http://opencontext.org) is probably our best bet there.

In the meantime however we've been chatting with Eric Poehler of the University of Massachusetts Amherst about his work at Pompeii, and he's provided us access to his very rich archive of site photographs. Given that there are few archaeological sites as well studied and well understood as Pompeii, these photos are excellent training data for us to work with. There is a good degree of ground truth. We'll work with Eric and his team then to develop our methods, which will also involve building some classifiers (using transfer learning) and image similarity visualizations at scale.

It has been a productive term, and I'm excited to see where Jeff takes this work next!
