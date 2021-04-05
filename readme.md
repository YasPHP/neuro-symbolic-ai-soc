# Neuro-Symbolic AI for Visual Question Answering

## Model
![NSAI VQA](https://cdn.discordapp.com/attachments/792469912295440438/828742534188630036/nsai.png)

## CVPR'20 Tutorial on Neuro-Symbolic Visual Reasoning and Program Synthesis
### Overview

Recent advances in deep learning gave rise to highly expressive models achieving remarkable results on visual perception tasks such as object, action and scene recognition. However, it is widely accepted that in order to develop truly intelligent systems, we need to bridge the gap between perception and cognition. Highly cognitive tasks such as planning, abstracting, reasoning and explaining are typically associated with symbolic systems which do not scale to the complex high-dimensional visual world. The relatively new field of neuro-symbolic computation proposes to combine the strengths of deep models with symbolic approaches, by using the former to learn disentangled, interpretable, low-dimensional representations which significantly reduce the search space for symbolic approaches such as program synthesis (cf. [5,15]). Another reason to study the interplay between neural and symbolic approaches is related to human, and in particular infant, learning. While far from fully understood, there is an increasing body of evidence that similar mechanisms combining low-level perception with high level cognition are at play in the human brain [1,12].

This tutorial will bring together researchers from computer vision, graphics, robotics, cognitive science, and developmental psychology to exchange ideas, share recent research results and applications in the emerging field of neuro-symbolic computation, focusing on computer vision.

- [Full Playlist](https://www.youtube.com/watch?v=Opunfo422uQ&list=PLX0h2D8LfCPHtT0-u6xjYaGFPT6-3cLJ1&index=1)


## Sort-of-CLEVR Dataset

Neuro-Symbolic AI allows us to combine Deep Learning’s superior pattern recognition abilities with the reasoning abilities of symbolic methods like program synthesis. This repository is an implementation of NSAI for Visual Question Answering on the Sort-of-CLEVR dataset using PyTorch. This implementation is inspired by the [Neuro-Symbolic VQA](https://arxiv.org/abs/1810.02338) paper by MIT-IBM Watson AI Lab.

The basic idea behind using NSAI for VQA is parsing the visual scene into a symbolic representation and using NLP to parse the query into an executable program which the program executor can use on the scene to find the answer. This implementation gets more than 99% on the Sort-of-CLEVR dataset.

## Requirements
- PyTorch version 1.2 and above
- OpenCV
- dlib
- Scikit Learn
- Pandas
- Numpy

## Usage
- The Step-by-Step usage is in the [NSAI on Sort-of-CLEVR.ipynb](https://github.com/nerdimite/neuro-symbolic-ai-soc/blob/master/NSAI%20on%20Sort-of-CLEVR.ipynb) notebook from training the individual modules to plugging everything together to test it.
- You can easily run this repository using Colab <a href="https://colab.research.google.com/github/nerdimite/neuro-symbolic-ai-soc/blob/master/NSAI%20on%20Sort-of-CLEVR.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"/></a>
- To understand more about the design and workflow, check out [NSAI Flow Diagram.pdf](https://github.com/nerdimite/neuro-symbolic-ai-soc/blob/master/NSAI%20Flow%20Diagram.pdf) which contains the workflows of every component i.e. Perception Module, Semantic Parser and Program Executor.

## References
- [Neural-Symbolic VQA: Disentangling Reasoning from Vision and Language Understanding](https://arxiv.org/abs/1810.02338)
- [The Neuro-Symbolic Concept Learner: Interpreting Scenes, Words, and Sentences From Natural Supervision](https://arxiv.org/abs/1904.12584)
- [Seq2Seq_Transformer](https://github.com/aladdinpersson/Machine-Learning-Collection/blob/master/ML/Pytorch/more_advanced/seq2seq_transformer/seq2seq_transformer.py)
- [Gesture Control](https://www.learnopencv.com/training-a-custom-object-detector-with-dlib-making-gesture-controlled-applications/)

## People
- [Kexin Yi](https://github.com/kexinyi)
- [Jiajun Wu](https://jiajunwu.com/)
- [Chuang Gan](https://people.csail.mit.edu/ganchuang/)
- [Antonio Torralba](https://www.csail.mit.edu/person/antonio-torralba)
- Pushmeet Kohli
- Joshua B. Tenenbaum
