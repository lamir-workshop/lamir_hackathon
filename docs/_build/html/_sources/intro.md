LAMIR 2024 Hackathon
====================================================

**By Matthew E. P. Davies, Sebastian Böck, Magdalena Fuentes**


<!-- ```{image} assets/placeholder.png
---
alt: Placeholder image to illustrate what are we talking about.
``` -->

Welcome message
---------------

Welcome to the website for the LAMIR 2024 Hackathon tutorial on Tempo, Beat, and Downbeat Estimation.

The highly interrelated topics of tempo, beat, and downbeat estimation from musical 
audio signals have spanned the entire history of MIR. Along with many MIR topics, the 
uptake of deep learning has fundamentally altered how these rhythm-oriented tasks have 
been addressed and has led to a profound increase in performance. This tutorial seeks to 
position itself within this narrative by providing a high-level understanding of 
historical signal processing-oriented approaches leading to hands-on practical 
experience in building, training, and evaluating the most recent state-of-the-art deep 
learning approaches. Our goal is not only to expose participants to a complete rhythm 
analysis pipeline, but also to emphasize the importance of technical and musical design 
choices, the reliability of annotated data, and multidisciplinarity. In addition, we 
seek to provide insight into common pitfalls and discuss future challenges.

The tutorial is targeted towards those in the LAMIR community who wish gain 
comprehensive insight and practical experience in tempo, beat, and downbeat estimation 
of musical audio signals. For those new to this area, we seek to provide a hands-on 
technical and pedagogical guide which can serve as the basis for fostering future 
research. For those with prior knowledge in the area, we hope to convey a solid 
understanding of recent advances and current state-of-the-art approaches. As a 
prerequisite for participation, we would expect some basic experience in the execution 
of python notebooks.


**For those who want to get straight to it...
all of the main practical code examples can be found 
in the following Google Colab notebook:** 


[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1tuOqNyO9gdMmYJsj33fP_QOfpRsm2tmt?usp=sharing)





Desired outcomes
----------------

The content of the LAMIR 2024 Hackathon has been organised in the form of an online 
book which we hope will remain a useful resource for the LAMIR community beyond
the LAMIR 2024 conference. By participating in the Hackathon directly, or following
the material offline, we strive for everyone to come away with the following:

* A high-level understanding of adapting deep learning models for music tasks in culturally diverse settings, focusing on meter tacking and source separation for Latin American music genres.
* Insights into the challenges and opportunities of applying MIR techniques to non-Western music, highlighting the importance of adapting models with minimal data.
* Knowledge of practical strategies like transfer learning, data augmentation, and fine-tuning, and their impact on model adaptability and performance.
* Familiarity with using existing datasets to address specific MIR tasks in music traditions that are often overlooked by mainstream research.

Via hands-on coding examples in python, we intend to provide practical experience in:
* Loading and processing datasets that include rhythmic instruments from Latin American traditions.
* Generating artificial mixtures from solo tracks and using these mixtures for training models.
* Adapting beat and downbeat tracking models using small annotated datasets and evaluating the models' performance.
* Exploring the capabilities of different model configurations, including deep learning-based TCNs and simpler statistical models, for musical analysis.


## Contributions from the community
We are happy to receive contributions to keep the resources and relevant works sections up-to-date. Please open an issue 
or submit a Pull Request in the main repository!


How to reference this book
--------------------------

**License**

```
@book{tempobeatdownbeat:book,
	Author = {Matthew E. P. Davies, Sebastian B\:ock, Magdalena Fuentes},
	Month = Nov.,
	Publisher = {https://tempobeatdownbeat.github.io/tutorial/intro.html},
	Title = {{Tempo, Beat and Downbeat Estimation}},
	Year = 2024,
	Url = {https://tempobeatdownbeat.github.io/tutorial/intro.html}
}
``` 
