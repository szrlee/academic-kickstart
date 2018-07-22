+++
title = "Learning Multi-channel Influence in Networks"
date = 2017-06-30T00:00:00
draft = false

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Yingru Li"]

# Publication type.
# Legend:
# 0 = Uncategorized
# 1 = Conference paper
# 2 = Journal article
# 3 = Manuscript
# 4 = Report
# 5 = Book
# 6 = Book section
publication_types = ["4"]

# Publication name and optional abbreviated version.
publication = "*Undergraduate Research Thesis*"
publication_short = "*Undergrad. Thesis*"

# Abstract and optional shortened version.
abstract = "Many social phenomena, such as the spread of diseases, behaviors, technolies, or products, an naturally be modeled as the diffusion of a contagion across a network. Owing to the potentially high social or economic value of accelerating or inhibiting such diffusions, the goal of understanding the flow of information and predicting information cascades has been an active area of research. In this context, a key task is learning and predicing social influence. Existing methods are based on classical influence models with large amounts of parameters, thus easily overfitted without massive data. Besides, these models rarely consider that diffusion of influence between two entities in network can be caused by multiple reasons: In social network, users can propagate information and influence via multiple communication channels; in disease network, disease can be infected by different ways including air, water, food; in bio-network, e.g. PPI network, proteins connect with each other through multiple pathways. We abstract these phenomena as **multi channel influence**. Since multiple channels are possibly co-existence, in this scenario, the final influence may be a nonlinear combination of the influence from every possible channels, instead of simply a linear combination. In this paper, we mainly study the *noisy-or-like* nonlinear combination of multi-channels influence."
abstract_short = "Many social phenomena, such as the spread of diseases, behaviors, technolies, or products, can naturally be modeled as the diffusion of a contagion across a network. Owing to the potentially high social or economic value of accelerating or inhibiting such diffusions, the goal of understanding the flow of information and predicting information cascades has been an active area of research. In this context, a key task is learning and predicing social influence..."

# Featured image thumbnail (optional)
image_preview = ""

# Is this a selected publication? (true/false)
selected = true

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's filename without extension.
#   E.g. `projects = ["deep-learning"]` references `content/project/deep-learning.md`.
#   Otherwise, set `projects = []`.
projects = ["social-network"]

# Tags (optional).
#   Set `tags = []` for no tags, or use the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = ["social-network-analysis", "hidden-structure", "social-influence", "machine-learning", "bayesian-network", "graphical-model"]

# Links (optional).
url_pdf = "files/papers/Thesis-MultiChanLearn.pdf"
url_preprint = ""
url_code = ""
url_dataset = ""
url_project = ""
url_slides = ""
url_video = ""
url_poster = ""
url_source = ""

# Custom links (optional).
#   Uncomment line below to enable. For multiple links, use the form `[{...}, {...}, {...}]`.
# url_custom = [{name = "Custom Link", url = "http://example.org"}]

# Does this page contain LaTeX math? (true/false)
math = true

# Does this page require source code highlighting? (true/false)
highlight = true

# Featured image
# Place your image in the `static/img/` folder and reference its filename below, e.g. `image = "example.jpg"`.
[header]
image = "headers/social-influence-wide.jpg"
caption = ""

+++
$$
\newcommand{\ChannelNum}{{l}}
\newcommand{\NodeNum}{{n}}
\newcommand{\EdgeNum}{{m}}
\newcommand{\CascNum}{{M}}
$$

Results show that under the network size of $\NodeNum$ and the node degree of $d$ with $\ChannelNum$ channels, the lower bound of sample complexity on Network Inference problem of some multi-channel models is $\Omega( d\log nl)$, which is proved with two different methods and is asymptotically equal to the resultof $\Omega( d\log n)$ for classical models since $l$ is always a constant. This complexity result indicates that introducing multi channel constraint do not increase the intrinsic complexity of solving network inference problems. Research also shows the influence function class under multi-channel independent cascade model are PAC learnable and the sample complexity is $\CascNum = \tilde{O}({\epsilon}^{-2}\NodeNum^3 \ChannelNum)$, which is not related to the number of the edges, much lower than the sample complexity of that under classical models. We finally give several solutions for network inference problem including frequency statistics, Maximum likelihood estimation and its sparsity version, which shows that introducing prior of multi-channel with \emph{noisy-or} combined effect help reduce the dimensionality of parameter space of influence model and improve the robustness of the algorithms. We also have proposed some potential models on continuous-times multi-channel influence behaviors and then consider modeling online dynamic networks as a future direction.

We concluded with following statements: the \emph{combined effect} can be effectively expressed using the \emph{Noisy or} non-linear model; considering multi channel phenomenon do not increase the intrinsic complexity of network inference problems and introducing the prior of multi channel with noisy-or combination can help reduce the complexity of learning influence functions.