---
title: Meta-learning in Robotic Manipulation
summary: "In top-5 among 46 projects in the course @ CMU 11-785 - Introduction to Deep Learning (Fall 2020) - [Project Gallery](https://deeplearning.cs.cmu.edu/F20/gallery/gallery.html)"
tags:
- Deep Learning
date: "2020-12-09T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Reach Task in Coppeliasim 
  focal_point: Smart

# links:
# - icon: twitter
#   icon_pack: fab
#   name: Follow
#   url: 
url_code: "https://github.com/Team-Grasp/idl-project"
url_pdf: "media/Team28.pdf"
url_slides: "https://slides.com/rohanpandya-1/deck"
url_video: "https://www.youtube.com/watch?v=cp1g_qhH-Go&feature=youtu.be"

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

_In top-5 among 46 projects in the course @ CMU 11-785 - Introduction to Deep Learning (Fall 2020) - [Project Gallery](https://deeplearning.cs.cmu.edu/F20/gallery/gallery.html)_

Reinforcement learning (RL) is a powerful learning technique that enables agents to learn useful policies by interacting directly with the environment. While this training approach doesn’t require labeled data, it is plagued with convergence issues and is highly sample inefficient. The learned policies are often very specific to the task at hand and are not generalizable to similar task spaces. 

Meta-Reinforcement Learning is one strategy that can mitigate these issues, enabling robots to acquire new skills much more quickly. Often described as “learning how to learn”, it allows agents to leverage prior experience much more effectively. Recently published papers in Meta Learning show impressive speed and sample efficiency improvements over traditional methods of relearning the task for slight variations in the task
objectives. A concern with these Meta Learning methods was that their success was only achieved on relatively small modifications to the initial task. 

Another concern in RL, as highlighted by [Henderson et al.](https://arxiv.org/abs/1709.06560), is reproducibility and lack of standardization of the metrics and approaches, which can lead to wide variations in reported vs observed performances. To alleviate that, benchmarking frameworks such as [Meta-World](https://arxiv.org/abs/1910.10897) and [RLBench](https://arxiv.org/abs/1909.12271) have been proposed that establish a common ground for a fair comparison between approaches. In this work, we aim to utilize the task variety proposed by [Meta-World](https://arxiv.org/abs/1910.10897) and compare PPO, a vanilla policy gradient algorithm, with their Meta Learning counterparts (MAML and Reptile). The objective is to verify the magnitude of success of meta-learning algorithms over the vanilla variants, and test them on a variety of complicated tasks to test their limits in responding to the size of task variations. We also introduce a new technique — Multi-headed Reptile, which proposes a novel approach to address some of the shortcomings of both these Meta-Learning techniques, with some computational implementation suggestions that prevent slowdown.