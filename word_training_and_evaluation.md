# Word-Based Training and Evaluation



### Reference

*   Convolutional Neural Networks for Small-footprint Keyword Spotting: https://www.isca-speech.org/archive/interspeech_2015/papers/i15_1478.pdf



## Training



**Not Obvious how to weight all of the different catgories.**

*   if no speech is present
*   if word been spoken that's not one it recognizes



Basic training idea:

*   Chosen words (10) + Unknown word (1) + silence / no speech detected (1)
*   data balancer and generator: 8.3% (= 100% / 12) for each category
*   `Unknown word` category randomly sampled from classes that are part of the target set
*   `silence (or no speech detected)` randomly sampled from background noise audio files
*   feature extraction: 
    *   40 dimensional log-me filter bank features 
    *   every 25ms with a 10ms frame shift
*   CNN for `small-footprint keyword spotting`



## Evaluation



*   **Top-1 Error** : similar with accuracy

*   **streaming error metrics**: confused to recognize the start or the end of words

















