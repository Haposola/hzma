---
permalink: /
title: "Hengzhao Ma"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am now working as an Assistant Professor, at Shenzhen Institute of Advanced Technology, Chinese Academy of Sciences. I received my bachelor and Ph.D. degree in the Department of Computer Science and Technology at Harbin Institute of Technology in 2016 and 2021, respectively. My research interests include computational theory, design, and analysis of algorithms for big data, and database technologies for AI. My current research focus is on vector similrity search.

A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, Academic Pages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

Publications
======
1. Hengzhao Ma, Jianzhong Li, Yong Zhang. Reconsidering Tree based Methods for k-Maximum Inner-Product Search: The LRUS-CoverTree. 40th International Conference on Data Engineering ICDE2024, Accepted)
1. Hengzhao Ma, Jianzhong Li. Turing Machines with Two-level Memory: New Computational Models for Analyzing the Input/Output Complexity[J]. Theoretical Computer Science, 2024, 985: 114347. 
1. Hengzhao Ma, Jianzhong Li. The Hardness of Optimization Problems on the Weighted Massively Parallel Computation Model[C]. The 29-th International Computing and Combinatorics Conference (COCOON), 2023: 106-117. 
1. Tianpeng Gao, Jianzhong Li, Hengzhao Ma. A New Approach for Semi-External Topological Sorting on Big Graphs[J]. IEEE Transactions on Knowledge and Data Engineering, 35(12), 12430-12443. 2023. 
1. Hengzhao Ma, Jianzhong Li, Xiangyu Gao, Tianpeng Gao. Turing Machines with Two-Level Memory: A Deep Look into the Input/Output Complexity[C]. The 28-th International Computing and Combinatorics Conference (COCOON), 2022: 199-211. 
1. Hengzhao Ma, Jianzhong Li. A Sub-linear Time Algorithm for Approximating k-Nearest-Neighbor With Full Quality Guarantee[J]. Theoretical Computer Science, 2021, 857: 59-70. doi: 10.1016/j.tcs.2020.12.039.
1. Hengzhao Ma, Jianzhong Li. An O(logn) query time algorithm for reducing ε-NN to (c,r)-NN[J]. Theoretical Computer Science, 2020, 803: 178-195. doi: 10.1016/j.tcs.2019.10.004. 
1. Hengzhao Ma, Jianzhong Li. A Sub-linear Time Algorithm for Approximating k-Nearest-Neighbor with Full Quality Guarantee[C]. The 14-th Annual International Conference on Combinatorial Optimization and Applications (COCOA), 2020: 19-31. Virtual,
1. Hengzhao Ma, Jianzhong Li. A True O(nlogn) Algorithm for the All-k-Nearest-Neighbors Problem[C]. The 13-th Annual International Conference on Combinatorial Optimization and Applications (COCOA), 2019: 362-374. Xiamen.
1. Hengzhao Ma, Jianzhong Li: An Algorithm for Reducing Approximate Nearest Neighbor to Approximate Near Neighbor with O(logn) Query Time[C]. The 12-th Annual International Conference on Combinatorial Optimization and Applications (COCOA), 2018: 465-479. Atlanta.
1. Anzhen Zhang, Jianzhong Li, Hong Gao, Yubiao Chen, Hengzhao Ma, Mohamed J. Bah. CrowdOLA: Online aggregation on duplicate data powered by crowdsourcing[J]. Journal of Computer Science and Technology, 2018, 33: 366-379.
1. 近似最近邻归约问题在泊松点过程上的再研究， 马恒钊，闫跃，李建中，软件学报，第34卷，第10期，4821-4829。


Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the Academic Pages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
