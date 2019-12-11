# Word-Level Audio Recognition


## Reference
* Tensorflow.js - Audio recognition using transfer learning
  * https://codelabs.developers.google.com/codelabs/tensorflowjs-audio-codelab/index.html#0
* Simple Audio Recognition
  * https://github.com/tensorflow/docs/blob/master/site/en/r1/tutorials/sequences/audio_recognition.md
* Pete Warden (2018) Speech Commands: A Dataset for Limited-Vocabulary Speech. arXiv:1804.03209v1

## Content

* Word-based Audio Data Processing: [markdown](word-based_preprocessing.md)
* Word-Based Training and Evaluation: [markdown](word_training_and_evaluation.md)

## Quick Start

The following is a way to demonstrate examples of this repository.
* `example_1_word_recognition`: a simple example for word-level audio recognition
* `example_2_retrain`: a simple example for retraining a model recognizing the words left, right and noise (blank).

```sh
git clone https://github.com/jiankaiwang/word_level_audio_recognition.git

# run the first example
cd example_1_word_recognition
python3 -m http.server

# run the second example
cd example_2_retrain
python3 -m http.server
```