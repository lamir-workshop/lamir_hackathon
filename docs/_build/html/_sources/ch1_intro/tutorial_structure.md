Tutorial structure and setup
============================

```{note}
The content in this section draws heavily from the excellent example
from the ISMIR 2020 tutorial:
[`Open Source Tools & Data for Music Source Separation`](https://source-separation.github.io/tutorial/landing.html)
```

## How to Use This Website

On the left-hand side of this web page you'll see the table of contents for the
entire tutorial. If you don't see the contents, click the hamburger (&#9776;) icon
to expand the left-hand column. On the right-hand side of the page you'll see 
the table of contents for this particular page. To navigate to the next section
you can either click on the next section on the tutorial's table of contents on 
the left-hand side, or you can scroll to the bottom of the page to click the 
button on the bottom right to go to the next section.


### Running Locally

<!--
```{figure} ../images/intro/run_local.gif
---
alt: There are links to download each notebook at top right of the page.
width: 600px
align: center
name: run-local
---
There are links to download each notebook at top right of the page.
```
-->

We have included links to our [github repo](https://github.com/TempoBeatDownbeat/tutorial)
which has `requirements.txt` to set up your own environment
so that you can use these tools locally, if you so choose. To run the notebook
locally, select ".ipynb" ("Download Source File") from the downloads drop down
menu at the top right corner of the page.

If you choose to run locally, here are the recommended steps:

1) Clone the [github repo](https://github.com/TempoBeatDownbeat/tutorial) into a 
   new directory.
2) Make a new conda environment.
    - If you want to install using `pip`, activate your environment and the
  run `pip install -r requirements.txt`. Note that you should have `ffmpeg` installed
  prior to installing the requirements ([instructions here](https://ffmpeg.org/download.html)).
3) Run `jupyter lab` in your command line and navigate to the URL that it prints
  in the console  
  ([instructions here](https://jupyterlab.readthedocs.io/en/stable/getting_started/starting.html)).
4) Learn!  


## Getting in Touch

### Github

<!--
```{figure} ../images/intro/github.gif
---
alt: Links to the Github repository are on the top right of the page.
width: 600px
align: center
name: github-links
---
Links to the Github repository are on the top right of the page.
```
-->

There are links to the Github repository for this website and its notebooks at
the top right corner of every page of this site. 

#### Found a bug? Typo?

Feel free to [open an issue here](https://github.com/TempoBeatDownbeat/tutorial/issues).
This link is also at the top right corner of every page.

```{note}
Especially for those participating in the live tutorial, we'll
almost surely need to iron out a few kinks in the days
immediately after we're done. So do watch out for updates
if something doesn't quite work as it should.
```


## Let's get started!

Press the button on the bottom right to advance to the next section.

# Tutorial scope and prerequisites

The scope of the material presented in the tutorial can be addressed in two ways: 
**technical** and **musical**.

From the **technical perspective** our primary focus is in providing hands-on experience
of current state of the art deep learning approaches.
To this end, we depart from historical signal processing approaches and move quickly 
from these into deep learning based approaches. 
In this way, we only touch upon the broader, multi-disciplinary context of the phenonema 
of the rhythmic and metrical structure of music and limit insights in relation to music 
cognition, computational neuroscience, and music theory. In sum, this tutorial can be 
primarily understood as a _data-driven_ approach to the estimation of tempo, beat, and downbeats from musical audio signals. 

It is important to note that this tutorial 
is **not** intended to be exhaustive in its coverage of all existing approaches, 
and furthermore places greater emphasis on more recent research covering the last
5 - 10 years. 

```{tip}
For anyone wanting a more detailed look at earlier approaches
we highly recommend the ISMIR 2006 tutorial on [Computational Rhythm Description](https://www.eecs.qmul.ac.uk/~simond/pub/2006/ISMIR06-RhythmTutorial-GouyonDixon.pdf) conducted by not one but **two**
former ISMIR Presidents: Fabien Gouyon and Simon Dixon.  
```

From the **musical perspective** we also restrict ourselves largely to musical content 
from a Western perspective. This is in no way an attempt to diminish or downplay the 
importance of non-Western musical traditions, but rather it is a reflection of the
knowledge-base and backgrounds of the presenters. 

Concerning **prerequisites** for this tutorial, some technical expertise
in the execution of python notebooks would be beneficial, although
it should be possible just to click through all of the examples
without that. In addition, we rely on some basic informal understanding
of metrical structure in music. In structuring the content of the 
tutorial, we have strived for a fairly light-weight and non-technical
introductory part, followed by some important theoretical constructs
concerning deep learning approaches to rhythm analysis,
prior to the main "hands-on" component. 

