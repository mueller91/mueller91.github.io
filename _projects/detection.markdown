---
layout: page
title: Deepfake detection
description: AI-driven audio deepfake detection and human perception
img: /assets/img/hacker.jpg
importance: 2
category: work
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" 
        src="{{ '/assets/img/demo_on_mac_c.jpg' | relative_url }}" alt="" 
title="example image"/>
    </div>
</div>

<br/>

We saw <a href="/projects/creation">earlier</a> that deep learning is able to clone the voice of any given target,
such as Angela Merkel.
This raises the following questions:
- How well are humans fooled by these deepfakes?
- Can we use AI to detect audio deepfakes?

We conducted an online study, where we presented over 8900 audio files to 200 users.
Each of the audio files was either authentic, or a deepfake.
The users were tasked with classifying the audio correctly as either authentic or deepfake. You can <a 
href="https://deepfake-demo.aisec.fraunhofer.de">try it yourself on this website</a>.
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
<div class="caption">
    The results of the Human vs. AI contest in audio deepfake detection. The leftmost image shows the Accuracy (i.e. the percentage of correct guesses) of the AI. The middle figure shows the Accuracy of all human players, averaged. The rightmost image shows the difference in Accuracy between the AI and the humans. Note that for all but one of the attacks (A7, A8, ..., A19) and the benign data (denoted by '-'), the AI outperforms the human players.
</div>

The AI outperforms the human players in all but one attack scenario. We interpret these results as follows:
- AI has a clear advantage over humans in the domain of audio deepfake detection.
- Still, in some cases, humans outperform the AI.

For more information, read our <a href="https://arxiv.org/pdf/2107.09667.pdf">paper</a>, on which this blog post is based.
