Title: The Big Data Brain Drain: Why Science is in Trouble
date: 2013-10-26 13:00
comments: true
slug: big-data-brain-drain

<!-- PELICAN_BEGIN_SUMMARY -->
Regardless of what you might think of the ubiquity of the "Big Data" meme, it's clear that the growing size of datasets is changing the way we approach the world around us.  This is true in fields from industry to government to media to academia and virtually everywhere in between. I come from a scientific research background, specifically in astronomy and astrophysics, and I've seen first-hand the power of data-centered methodology in deciphering the mysteries of the Universe. Our increasing abilities to gather, process, visualize, and learn from large datasets is helping to push the boundaries of our knowledge.

But, where scientific research is concerned, this recently accelerated shift to data-centered science has a dark side, which boils down to this: the skills required to be a successful researcher are increasingly indistinguishable from the skills required to be successful in industry. While academia, with typical inertia, gradually shifts to accommodate this, the rest of the world has already begun to embrace and reward these skills to a much greater degree. *The unfortunate result is that some of the best and brightest upcoming researchers are finding no place for themselves in the academic community, while the for-profit world of industry stands by with deep pockets and open arms.*
<!-- PELICAN_END_SUMMARY -->

The Unreasonable Effectiveness of Data
--------------------------------------
In 1960, the physicist Eugene Wigner published his famous essay, [*The Unreasonable Effectiveness of Mathematics in the Natural Sciences*](http://en.wikipedia.org/wiki/The_Unreasonable_Effectiveness_of_Mathematics_in_the_Natural_Sciences).  It expounds on the surprising extent to which abstract mathematical concepts seem to hold validity in contexts far beyond those in which they were developed. After all, who would have guessed that Riemann's 19th century studies in non-Euclidean geometry would form the basis of Einstein's rethinking of gravitation, or that a codification of the rotation groups of abstract solids might eventually lead Physicists to successfully predict the existence of the Higgs Boson?

Echoing this, in 2009 Google researchers Alon Halevy, Peter Norvig, and Fernando Pereira penned an article under the title [*The Unreasonable Effectiveness of Data*](http://static.googleusercontent.com/external_content/untrusted_dlcp/research.google.com/en/us/pubs/archive/35179.pdf).  In it, they describe the surprising insight that given enough data, often the choice of model stops being important &mdash; that "correct" models reflecting deep insight into a problem are superfluous given a large enough dataset. Using Google's language translation software as a case study, they make the case that "simple models and a lot of data trump more elaborate models based on less data."

If we make the leap and assume that this insight can be at least partially extended to fields beyond natural language processing, what we can expect is a situation in which domain knowledge is increasingly trumped by "mere" data-mining skills. I would argue that this prediction has already begun to pan-out: **in a wide array of academic fields, the ability to effectively process data is superseding other more classical research methods.**

Now, I'm not arguing here that domain understanding is entirely obsolete; after all the [10GB/second](http://home.web.cern.ch/about/computing) produced by the Large Hadron Collider (LHC) would be virtually useless apart from a solid theoretical understanding of the particle interactions that produce them, just as the [15TB/night](http://www.lsst.org/lsst/public/tour_software) of raw image data produced by the Large Synoptic Survey Telescope (LSST) would have very little to tell us about cosmology absent our theoretical insight into the physical processes driving the expansion of the Universe.  But the LHC and LSST reflect the increasingly common situation where scientific results are entirely dependent upon the use of sophisticated methods to analyze large datasets. Indeed, we're finding that even when the data don't quite qualify as "Big", progress in science is increasingly being driven by those with the skills to manipulate, visualize, mine, and learn from data.

The New Breed of Scientist
--------------------------
In some senses, the age of data-driven research has not significantly changed the academic milieu. Since we shed Aristotelianism in the 16th-17th centuries, scientific progress has been largely based on empirical experiment and observation.  It was Tycho Brahe's unprecedented 16th-century survey of the sky, after all, that led to Kepler's 17th century Laws of planetary motion, and paved the way for Newton's Universal Law of Gravitation and eventually Einstein's General Theory of Relativity.  Scientists have always grappled with data; the difference is that today this act of grappling is increasingly central to the scientific process.

The increasing data-centeredness of science, however, is already leading to new approaches to problems: in the era of the LHC and LSST, the most exciting research is being driven by those who have the expertise to apply high-performance data-parallel statistical algorithms to ask interesting questions of huge, community-generated datasets.  It is driven by the application of new statistical approaches, of new machine learning algorithms, and of new and faster codes to repeat classic analyses at a previously unattainable scale.  **In short, the new breed of scientist must be a broadly-trained expert in statistics, in computing, in algorithm-building, in software design,** and (perhaps as an afterthought) in domain knowledge as well. From particle physics to genomics to biochemistry to neuroscience to oceanography to atmospheric physics and everywhere in-between, research is increasingly data-driven, and the pace of data collection shows no sign of abating.

The Fundamental Role of Scientific Software
-------------------------------------------
The common thread here is that of scientific software: none of this work happens without the writing of code.  And unless that code is well-written, well-documented, and shared openly with the community, the reproducibility paramount to the scientific process will be threatened. Much has been written about the current [crisis of irreproducibility](http://phys.org/news/2013-09-science-crisis.html) in science, about the need for [new forms](http://python.6.x6.nabble.com/IPython-Notebooks-dissertations-and-scholarly-publication-td5036272.html) of [publication](http://www.elsevier.com/connect/executable-papers-in-computer-science-go-live-on-sciencedirect), and new [openness of access](http://www.openscience.org/blog/?p=686) to research, code, and data.  I won't dwell on those issues here.

What I will dwell on is the central role of optimized, specialized software in the analysis and visualization of large datasets, and the direct translation of that to its central role in modern scientific research. My collaborator Gael Varoquaux and his colleagues recently published an [editorial](http://hal.inria.fr/hal-00858663/en) arguing this point (see Gael's short summary [here](http://gael-varoquaux.info/blog/?p=170)), and making the case that **open, well-documented, and well-tested scientific code is essential not only to reproducibility in modern scientific research, but to the very progression of research itself.** New research cannot build upon past results if those results are simply mentioned in a paper, with the actual process of producing them trapped in undocumented code hidden somewhere in somebody's laptop. As [Buckheit and Donoho](http://www-stat.stanford.edu/~wavelab/Wavelab_850/wavelab.pdf) have written,

> An article about computational science in a scientic publication is not the scholarship itself, it is merely advertising of the scholarship. The actual scholarship is the complete software development environment and the complete set
of instructions which generated the figures.

Though I may not have expressed it so eloquently, I realized early in my graduate career the paramount importance of sharing and maintaining scientific code.  This is what has led me to invest so much of my time in the development and support of open-source tools like Scikit-Learn, SciPy, NumPy, Matplotlib, IPython, and other pieces of the scientific Python ecosystem.

Academia's Disconnect
---------------------
This brings us to Academia's core problem: despite the centrality of good software to the current paradigm of scientific research, **academia has been singularly successful at discouraging these very practices that would contribute to its success.**  In the "publish-or-perish" model which dominates most research universities, any time spent building and documenting software tools is time spent *not* writing research papers, which are the primary currency of the academic reward system.  As a result, except in certain exceptional circumstances, those who focus on reproducible and open software are less likely to build the resume required for promotion within the academic system.  And those poor souls who have a gift for scientific software development rather than the writing of research papers will mostly find themselves on the margins of the academic community.

To an extent, this has always been the case.  The academic system has always rewarded some skills at the expense of others: for example, teaching skills are one area which seem to be perenially overlooked.  But there are two main differences that come up within the current discussion:

1. As I've mentioned, the skills now slipping through the cracks of the academic reward structure are the very skills required for the success of modern research.

2. With virtually the entire world utilizing the tools of data-intensive discovery, the same skills academia now ignores and devalues are precisely the skills which are most valued and rewarded within industry.

The result of this perfect storm is that skilled researchers feel an insidious gradient out of research and into industry jobs. While software-focused jobs do exist within academia, they tend to be lower-paid positions without the prestige and opportunity for advancement found in the tenure track.  Industry is highly attractive: it is addressing interesting and pressing problems; it offers good pay and benefits; it offers a path out of the rat-wheel of temporary postdoctoral positions, and often even encourages research and publication in fundamental topics.  Most importantly, perhaps, **industry offers positions with a real possibility for prestige and career advancement.**  It's really a wonder that any of us stay in the academy at all.

I particularly worry about this in my own field.  The [LSST project](http://www.lsst.org/) is ramping up for first-light toward the end of this decade. To handle the volumes of data involved, the project will likely be looking to hire several dozen data-focused researchers.  Given the required skill set, along with the current compensation level and career outlook of positions like these, I have some serious doubts about whether the project will be able to attract a sufficient pool of applicants for these positions.

How should Academia Adapt?
--------------------------
I'm in no way the only person thinking about these issues.  I've discussed pieces of this topic with many folks from around the country and the world, and I know that there are funding agencies thinking about these very problems. But the practical question of how to address these concerns looms large.  Complaining about the culture of academia seems to be a common past-time of academics: some of what I'm saying here echos Deirdre McCloskey's *Law of Academic Prestige*: "the more useful the field, the lower its prestige".  Though this was originally coined in lamentation of the low status of essential topics like freshman writing and composition, it seems readily applicable to the current subject.

I would argue that the concept of prestige is the key: the solution to the problem lies in taking deliberate measures within academia to catch-up with industry and increase the prestige of those who work to develop the software tools essential to current data-driven scientific research.  There are a few specific things that researchers, funding agencies, and policy leaders can do to promote this.  Here are a few ideas:

1. **Continue to press the importance of reproducibility in academic publication**. Not only is this absolutely essential to the scientific process itself, but reproducibility depends on open, documented, and well-written code. Making this code an essential part of published research will make those with software skills an essential part of the academic community.

2. **Push for a new standard for tenure-track evaluation criteria**: one which considers the creation and maintenance of open software along with more traditional activities like publication and teaching.  This will remove a main disincentive against spending energy on producing clean, well-documented, and open code.

3. **Fund and create a new class of positions**, from graduate and post-doctoral fellowships to research faculty, teaching faculty, and tenure-track faculty.  These positions should particularly emphasize and reward the development of open, cross-disciplinary scientific software tools.  Positions like these would present a viable academic career path for those interested in building and maintaining the essential software used by themselves and their colleagues.

4. **Increase the pay of post-doctoral scientific research positions.**  Some might find this idea controversial, but the current situation is absolutely unsustainable.  The base postdoctoral salary for NIH positions is [under $40,000 per year](http://grants.nih.gov/grants/guide/notice-files/NOT-OD-12-033.html) for someone who has just completed a PhD in their field. This is generously increased to about $50,000 per year after seven (!) years of post-doctoral experience. Those with the skills mentioned in this article could easily ask for several times that compensation in a first-year industry job, and find themselves working on interesting problems where their computational skills are utilized and valued.

I fear that without these sorts of changes in the culture of academia itself, the progress of scientific research will be severeley handicapped in the coming years.

We live in an exciting time, where the depth and breadth of our scientific understanding of the world around us are being driven by an ever accelerating ability to gather, store, process, and learn from datasets of unprecedented size.  To keep up this pace of discovery, the best researchers need incentives to stay within the research community.  It's not an easy problem to address, but with a little effort, we can assure the health and sustainability of the scientific research community into the future.