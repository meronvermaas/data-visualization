---
title: Dataset 1
nav: true
---

# Filter and Fire Dataset

Let's get started using any of the examples mentioned in [preparation](0-prep.md).

The [Filter and Fire Dataset](https://www.kaggle.com/datasets/selfishgene/fiter-and-fire-paper) is part of a project whose aim is to explain what are the functional implications of the many synaptic contacts that have been observed between a cortical neuron and the dendrites of it's post-synaptic neuron. 

Here, the authors propose a 'Filter and Fire Neuron Model' (F&F), which, in contrast to the long-stablished 'Integrate and Fire Neuron Model' (I&F), takes into account the spatio-temporal information obtained from multiple synaptic contacts. To compare the efficacy of the different models, they tested the 'memory capacity' of the neurons by training the neurons in each model type to emit precisely-timed output spikes for a random input pattern, in this case, handwritten digits:

{% include figure.html img="FF_Fig3A.jpg" alt="Filter&Fire paper Fig.3A" caption="from Fig.3A [Beniaguev, et al. bioRxiv 2024](https://doi.org/10.1101/2022.01.28.478132)" width="75%" %}

The Filter and Fire Dataset table contains the following information:
digit: handwritten digit used as imput pattern for training the neurons
M_connections: number of connections per neuron
Time: temporal interval
Accuracy.baseline: Baseline accuracy to detect a digit for a neuron before training
Accuracy.FF: accuracy of produced spikes after training for detecting a digit under the Filter and Fire model

| digit    | M_connections | Time    | Accuracy.baseline | Accuracy.FF |
| -------- | ------------- | ------- | ----------------- | ----------- |
| 7  | 5    |  60  | 94.44000  | 89.72   |
| 3 |   5   |  60  | 94.71000  | 90.42    |
| 1    | 5    |  30  | 89.93667	 | 89.90  |


Now we can go on an visualize our data!

Follow one R or Python Notebook to obtained the code used to generate the following plots:

