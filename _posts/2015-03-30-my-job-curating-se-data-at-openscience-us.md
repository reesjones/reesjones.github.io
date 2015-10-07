---
layout: post
title: My Job - Curating SE Data at openscience.us
---

Back in January, I started a part-time job at N.C. State, joining my colleague and good friend [Carter Pape](https://github.com/CarterPape) in developing version 4 of [openscience.us/repo](http://openscience.us/repo), a long-term repository for software engineering (SE) research data. I wasn’t too knowledgeable about what I was getting into, but through the past few months I’ve gained some insight into the philosophy of SE research – and how [Dr. Tim Menzies](http://menzies.us/) and his brainchild OpenScience is making software engineering research a more reproducible and replicable process.

## Software Analytics

Software analytics deals with the analysis of data gathered from software engineering to gain insights that can produce actionable advice to improve software engineering. Such advice can include using

 * XML descriptions of design patterns to recommend particular designs [1],
 * software process models to learn effective project changes [2], and
 * bug databases to learn defect predictors that guide inspection teams to where the code is most likely to fail [3-5].

A common problem associated with software analytics, which includes SE research, is that many research papers that used SE data to reach conclusions is not provided with the paper. An essential paradigm of the scientific method is that results must be both *reproducible* and *replicable*. Reproducibility is the ability to reproduce an experiment; e.g. take somebody’s previous experiment and rerun it with either their data or on your own data (it depends on who you ask – the precise definition is a bit fuzzy). Replicability is achieved when the same results are gathered from the *same* experimental methods with the *same* data.

So…when the data used in a particular study or experiment is not provided to the academic community, the study or experiment is irreproducible and therefore irreplicable. There’s solid evidence of this, as stated on the [openscience.us/ssj/manifesto](http://openscience.us/ssj/manifesto) page:

> There are very few replications of prior SE results. For example, in 2010, [Robles](http://v.gd/kTm2Kz) published a retrospective study of the 171 papers published in the Mining Software Repositories (MSR) conference [106]. He found that over 95 of those papers were unreproducible, since their associated data was no longer on-line. This lack of availability of old MSR data was discussed, at length, at MSR 2013. According to those participants, the single biggest contributor to this issue was the lack of a free-to-use long-term storage facility for big files. For example, free services like GitHub or GoogleCode impose limits of just a few gigabytes on the total repository size.

So not only is some data not being published (therefore breaking the academic research model), but the data that is published tends to go missing over time. As the manifesto states, a reliable long-term storage repository for data simply didn’t exist. That’s where I come in!

## The tera-PROMISE repository

My job involves two main branches of work: developing the actual site with HTML, CSS, and the Jekyll framework, and curating/adding research data as it is submitted. It is also described in the OpenScience manifesto:

> **SOLUTION #4:** Create a large free-to-use repository for SE [research products](http://openscience.us/ssj/researchproducts.html). To this end, we have created a [large repository](https://terapromise.csc.ncsu.edu:8443/svn/repo) for storing the data, plus creating a [discussion site](http://openscience.us/repo/) for those contents calculate, that this repository requires one petabyte of storage.

So I work on building the actual site with [Jekyll](http://jekyllrb.com/), a “simple, blog-aware, static site generator”, and adding datasets to the site as Jekyll posts and uploading them to the SVN repository. The Jekyll site hosts the data descriptions and context notes to the data, along with a link to the data in the SVN repository, hosted separately at N.C. State University.

And that’s my job! There are currently over 100 datasets housed in the tera-PROMISE repository, some of which are circa 2004, sorted into 18 categories. If you happen to be a researcher who wants data to be uploaded, feel free to browse around the current projects and fill out a [Google Form](http://goo.gl/7mWybm) with the appropriate information. You can also email [openscience.content@gmail.com](mailto:openscience.content@gmail.com) if you prefer.
 

These references were gathered from [this IEEE article](http://ieeexplore.ieee.org/xpl/articleDetails.jsp?arnumber=6547619) on software analytics, co-authored by Dr. Menzies.

F. Palma, H. Farzin, and Y.-G. Gueheneuc, “Recommendation System for Design Patterns in Software Development: A DPR Overview,” Proc. 3rd Int’l Workshop Recommendation Systems for Software Eng., IEEE, 2012, pp. 1–5
D. Rodríguez et al., “Multiobjective Simulation Optimisation in Software Project Management,” Proc. Genetic and Evolutionary Computation Conf., ACM, 2011, pp. 1883–1890.
T. Menzies, J. Greenwald, and A. Frank, “Data Mining Static Code Attributes to Learn Defect Predictors,” IEEE Trans. Software Eng., Jan. 2007; http://menzies.us/pdf/06learnPredict.pdf.
T.J. Ostrand, E.J. Weyuker, and R.M. Bell, “Where the Bugs Are,” Proc. 2004 ACM SIGSOFT Int’l Symp. Software Testing and Analysis, ACM, 2004, pp. 86–96.
S. Kim et al., “Predicting Faults from Cached History,” Proc. Int’l Conf. Software Eng., IEEE CS, 2007, pp. 489-498.
