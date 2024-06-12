---
title: Dataset 1
nav: true
---

# Filter and Fire Dataset

Cortical neurons have long been observed to form multiple synaptic contacts with it's post-synaptic target. Yet, the functional advantages that arise with this increased number of contacts is still to be understood. 

[In this study](https://doi.org/10.1101/2022.01.28.478132), the authors propose a 'Filter and Fire Neuron Model' (F&F), which, in contrast to the long-stablished 'Integrate and Fire Neuron Model' (I&F), takes into account the spatio-temporal information obtained from multiple synaptic contacts. 

To compare the efficacy of the different models, they tested the 'memory capacity' of the neurons by training the neurons in each model type to emit precisely-timed output spikes for a random input pattern, in this case, handwritten digits:

{% include figure.html img="FF_Fig3A.jpg" alt="Filter&Fire paper Fig.3A" caption="from Fig.3A, Beniaguev, et al. bioRxiv 2024" width="75%" %}

The [Filter and Fire Dataset](https://www.kaggle.com/datasets/selfishgene/fiter-and-fire-paper) table contains the following information:

* digit: handwritten digit used as imput pattern for training the neurons
* M_connections: number of connections per neuron
* Time: temporal interval
* Accuracy.baseline: Baseline accuracy of a neuron to detect a digit (before training)
* Accuracy.FF: accuracy of produced spikes after training under the Filter and Fire model

| digit    | M_connections | Time    | Accuracy.baseline | Accuracy.FF |
| :------: | :-----------: | :-----: | :---------------: | :---------: |
| 7  | 5    |  60  | 94.44000  | 89.72   |
| 3 |   5   |  60  | 94.71000  | 90.42    |
| 1    | 5    |  30  | 89.93667	 | 89.90  |


Now we can go on an visualize our data!

Follow one R or Python tutorials to generate the following plots:

### Barplot

We can observe the Baseline Accuracy displayed by neurons for the detection of each handwritten digit by making a Bar plot.

Barplots are usefull for representing relationships between a numeric (in this case, the Baseline accuracy values) and a categorical variable (in this case, the handwritten digit pattern)

As mentioned on section "Color Theory in Graphs" of the Data Visualization handbook, color is an important element to aid with visualizing our data. Here, we have selected to use a different color for each one of the digits so we can easily visualize the differences between each one of them. 

{% include figure.html img="Barplot-R.png" alt="Barplot" caption="" width="75%" %}
