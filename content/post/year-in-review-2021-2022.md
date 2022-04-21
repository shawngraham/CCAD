---
title: "What Happened to 2021-2022?"
date: "2022-04-21"
tags: ["meta", "recap","image_recognition"]
---

## General Thrust of Our Group This Year

Last year, we moved to more of a skunkworks approach, where I provided some overall direction, but allowed the team to follow their nose where'er it leads. In general terms, we're taking an approach to using computer vision to archaeological imagery, for both research, outreach, and as a lens through which we deform the past, to bring new elements into view

## Graduates

+ Completed MA for Jeff Blackadar, History with Data Science. "AUTOMATED METHODS TO COLLECT HISTORICAL INFORMATION FROM LIDAR IMAGES AND MAPS."

Abstract: "In this thesis I use ‘deep learning’, a form of artificial intelligence, to detect features in landscapes and imagery that are of interest to historians. What’s more, I demonstrate reproducible workflows making these methods available to individual historians who do not have a background in machine learning. The first section of the case studies uses a custom trained deep learning model to detect relict charcoal hearths in LiDAR data of the Earth’s surface. The second section of case studies uses commercially available deep learning services to extract geolocated features from historical maps." Open notebook at http://jeffblackadar.ca/

+ Completed MA for Jaime Simons, Public History with Digital Humanities. "REMIXING THE OTTAWA:  SOUNDS, SENSATIONS, AND STEAMBOAT CONNECTIONS ON THE OTTAWA RIVER, 1823 to 1949"

Abstract: "For over a century, steamboats plied the Ottawa River. They facilitated the colonial settlement of the Ottawa Valley and supported the logging, mining, and railway industries. They were used for tourism and religious colonization schemes, and were both catalysts and aids for the restructuring of the river and the spreading of disease. Settler reliance on steamboats made them an invaluable piece of early industrial infrastructure, turning the Ottawa River into a water-based highway in the service of settler colonialism, resource extraction, and Indigenous dispossession.
This research essay and EP (Extended Play album), titled Remixing the Ottawa, uses sound and performance theory to engage with the history of steamboat imperialism on the Ottawa River. Through six audio tracks (Merging Temporalities, Rising Waters, Hearing Silence, Colonial Connections, ‘Authentic’ Excursions, and Hymns, Dispossession, and Disease), the EP represents and recreates these histories in the present, to re-forefront their forgotten impacts and hidden harms.
The project website can be found at https://jaimesimns.github.io/remixingtheottawa/"

## Publications

+ Graham, S, and Simons, J. 2021 Listening to Dura Europos: An Experiment in Archaeological Image Sonification, Internet Archaeology 56. https://doi.org/10.11141/ia.56.8

Abstract: "We present an experiment in sonifying archival archaeological imagery to make the act of looking at photography strange and weird. The sounds produced will then arrest us and slow us down, and make apparent to us the different ways that archaeological vision is constructed to particular effect/affect. It makes us alive to what is hidden or elided in the image itself; in slowing down, listening/looking/moving at one, we are moved towards enchantment, and engage in a kind of digital hermeneutics that reveals more than what the lens may have captured."

+ Carter, B., Blackadar, J., & Conner, W. (2021). When Computers Dream of Charcoal: Using Deep Learning, Open Tools, and Open Data to Identify Relict Charcoal Hearths in and around State Game Lands in Pennsylvania. Advances in Archaeological Practice, 1-15. [doi:10.1017/aap.2021.17](https://www.cambridge.org/core/journals/advances-in-archaeological-practice/article/when-computers-dream-of-charcoal/EE88E84ECC44E369B8FA002D7353FC2F)

Abstract: "This research employs machine learning (Mask Region-Based Convolutional Neural Networks [Mask R-CNN]) and cluster analysis (Density-based spatial clustering of applications with noise [DBSCAN]) to identify more than 20,000 relict charcoal hearths (RCHs) organized in large “fields” within and around State Game Lands (SGLs) in Pennsylvania. This research has two important threads that we hope will advance the archaeological study of landscapes. The first is the significant historical impact of charcoal production, a poorly understood industry of the late eighteenth to early twentieth century, on the historic and present landscape of the United States. Although this research focuses on charcoal production in Pennsylvania, it has broad application for both identifying and contextualizing historical charcoal production throughout the world and for better understanding modern charcoal production. The second thread is the use of open data, open source, and open access tools to conduct this analysis, as well as the open publication of the resultant data. Not only does this research demonstrate the significance of open access tools and data but the open publication of our code as well as our data allow others to replicate our work, to tweak our code and protocols for their own work, and reuse our results.""

+ Blackadar, Jeff, Benjamin Carter, and Weston Conner. “Object Detection Model, Image Data and Results from the ‘When Computers Dream of Charcoal: Using Deep Learning, Open Tools and Open Data to Identify Relict Charcoal Hearths in and Around State Game Lands in Pennsylvania’ Paper.” Journal of Open Archaeology Data 9 (December 27, 2021): 12. https://doi.org/10.5334/joad.81.

+ Blackadar, Jeff, Benjamin Carter, and Weston Conner. “RCH Detection with Mask R-CNN Images.” Zenodo, March 4, 2021. https://doi.org/10.5281/zenodo.4583945.

## Presentations

+ Presentation by Scott Coleman on RTI and Numismatics - Underhill Graduate Colloquium, Carleton University
+ Presentation by Kavita Mistry on Photogrammetry from Archival Photos - Underhill Colloquium, Carleton University

## Experiments Underway

At our intake meeting for this year, new students Noah Chapman, Kavita Mistry, and Scott Coleman decided they wanted to see if they could create creative, immersive, pedagogical experiences from legacy data. They are embarking on building a reproducible workflow for procedurally modeling built spaces from site plans, as they become known through trench notebooks and other ancillary records.

## On Our To-Do List

+ eye tracking on archival archaeological photos, like the ones from dura europos (Graham & Simons, 2021). The sonification just took three lines through each image at the same spot to sample data; but what if we sonified the data that people actually looked at? and do people read those old photos differently than they would contemporary archaeological photos?

+ The Imagination of the Machines. This paper is nearing completiong, and features 3d photogrammetric reconstructions of the latent space of computers trained to see like archaeologists.

## Archaeology in Space

How do you record archaeological data in space? On the ground, we understand and create archaeological knowledge by reading the positioning of materials in 3d space; broadly speaking, the depth dimension stands in as a proxy for time. That is to say, _gravity_ is fundamental for creating archaeological knowledge. But when you have no gravity? What then? In december, I was asked for ideas on how to develop a system for the International Space Station Archaeology Project to enable them to record material culture in-situ on the space station - the astronauts take photos, the archaeologists study them. I wrote about the system I cobbled together and which Chantal Brousseau then polished up and made workable on the [International Space Station Archaeology Project blog](https://issarchaeology.org/how-do-you-get-from-an-astronauts-photo-to-usable-archaeological-data/).

I want to repurpose this system to work with other kinds of 'weird' archaeology.  I have access to an orphaned archaeological collection from the Canadian Museum of Nature; in this case, it lacks context, not gravity. But maybe gravity and context are just synonyms? Anyway, I think this tool will be useful in this case and we're planning out an experiment.
