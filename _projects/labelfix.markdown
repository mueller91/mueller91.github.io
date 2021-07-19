---
layout: page
title: correctness of ML-datasets
description: identifying mislabeled instances in AI-datasets
img: /assets/img/dataset.png
importance: 3
category: work
---

Machine learning requires data from which to learn: 
Even the most advanced neural network $$f$$ is merely a mapping $$ x \to y $$, learnt from the training dataset.
Thus, the correctness of training data is paramount.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/cifar.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
	The Cifar-10 dataset (<a href="https://github.com/dnddnjs/pytorch-cifar10">Image Source</a>), consisting of 60.000 images corresponding to one of ten classes such as 'airplane', 'ship' or 'cat'.
</div>

However, it turns out that even in the most popular datasets, there are a number of instances whose labels $$y$$ are plain wrong.
Consider the following examples from the Cifar-10 dataset:

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/labelfix1.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
	Four mislabeled instances from the Cifar-10 dataset. The caption indicates the label and the ID of the instance in the dataset. Observe, for example, the small bottle (?) shown in the leftmost picture, which is labeled as a 'cloud'.
</div>

While the Cifar-10 dataset generally is very clean (we only found 7 mislabeled instances in 60.000 images),
other datasets contain a much larger number of mislabeled samples.
This is not just problematic for training, but also for evaluation, since it skews Accuracy and other metrics.

In our paper, we present a simple and straightforward algorithm to remedy this: Go have a 
<a href="https://arxiv.org/pdf/1912.05283.pdf">look</a>.