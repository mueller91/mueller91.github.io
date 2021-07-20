---
layout: page
title: Deepfake detection
description: How to identify audio-deepfakes
img: /assets/img/hacker.jpg
importance: 2
category: work
---

We saw <a href="/projects/creation">earlier</a> that deep learning is able to clone the voice of any given target,
such as Angela Merkel.
This raises the following questions:
- How well are humans fooled by these deepfakes?
- Can we use AI to detect audio deepfakes?

We conducted an online study, where we presented over 8900 audio files to 200 users.
Each of the audio files was either authentic, or a deepfake.
We then measured the performance of both the human players, as well as the performance of an AI specifically trained to detect audio deepfakes.

The following charts show the results:

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/ml_acc_by_attack_id.png' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/user_acc_by_attack_id.png' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/delta_acc_ai_human.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>