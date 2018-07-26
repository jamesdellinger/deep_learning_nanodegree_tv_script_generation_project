# Project: Generate a TV Script Using RNNs
*Training a recurrent neural network to create a script for a [Simpsons](https://en.wikipedia.org/wiki/The_Simpsons) scene that takes place in [Moe's Tavern](https://simpsonswiki.com/wiki/Moe's_Tavern).*

<img src="https://github.com/jamesdellinger/deep_learning_nanodegree_tv_script_generation_project/blob/master/dlndlogo.png" height="140">

For Udacity's [Deep Learning](https://www.udacity.com/course/deep-learning-nanodegree--nd101) Nanodegree.

Topic: Recurrent Neural Networks.

## Overview
* I built from scratch a recurrent neural network using LSTM cells, used TensorFlow to train it on a text dataset that is a compilation of scripts from several Simpsons TV shows, and then used this trained model to generate a brand new Simpsons script.
* My network learned on its own how a TV script should be formatted, as well as rules for grammar, syntax, and punctuation, along with a very basic grasp of the personalities of the different characters. Here's an excerpt:
  ```
  moe_szyslak: yeah on the ball thing.
  lenny_leonard: i see this for now since there who makes sense home she. while.
  carl_carlson: pick up! what?
  moe_szyslak: just what have money for the president of course that old friend, boxing i was! another moe
  barney_gumble: hey! what, you're the fat one else stupid(to, lenny homer? hey) they the should put on how a daddy? 'cause you sayin' you look, but that you've had all a feeling moe_szyslak: him for / yeah with the"
  ned_flanders: hey guys stink, usin'. it's husband at
  homer_simpson:(realizing at a man sorry homer then) there, didn't be" eightball" problem?!
  ```
* The dataset I used is a subset of the [The Simpsons by the Data](https://www.kaggle.com/wcukierski/the-simpsons-by-the-data) dataset that can be found on kaggle. It was originally compiled by [Todd W. Schneider](http://toddwschneider.com/posts/the-simpsons-by-the-data/).
* This subset consists only of Simpsons scenes that take place in [Moe's Tavern](https://simpsonswiki.com/wiki/Moe's_Tavern).

## Concepts
* RNNs and LSTM cells.
* TensorFlow dropout wrappers.
* Preprocessing a text dataset, building lookup tables, and tokenizing punctuation.
* Writing from scratch an algorithm to generate training batches.
* Building a network's computation graph using TensorFlow.
* My RNN included a word2vec embedding layer based on the [Skip-gram](http://mccormickml.com/2016/04/19/word2vec-tutorial-the-skip-gram-model/) architecture, and I trained my network to predict the word directly following each word in the training set.
* Tuning RNN hyperparameters like number of epochs, batch size, LSTM cell size, embedding layer dimension size, word2vec sequence length, and learning rate.
* Using a trained model to make predictions and generate completely new text content, starting with only a single prime word ('moe_szyslak' in this case).

## My Completed Project
* [ipython notebook](https://github.com/jamesdellinger/tv_script_generation_project/blob/master/dlnd_tv_script_generation.ipynb) / [html version](http://htmlpreview.github.com/?https://github.com/jamesdellinger/tv_script_generation_project/blob/master/dlnd_tv_script_generation.html) / [pdf version](https://github.com/jamesdellinger/tv_script_generation_project/blob/master/dlnd_tv_script_generation.pdf)

## Project Grading and Evaluation
* [Project Review](https://github.com/jamesdellinger/deep_learning_nanodegree_your_first_neural_network_project/master/tv_script_generation_project_review.pdf)

* [Project Grading Rubric](https://github.com/jamesdellinger/deep_learning_nanodegree_tv_script_generation_project/blob/master/tv_script_generation_project_grading_rubric.pdf)

## Dependencies
* [requirements.txt](https://github.com/jamesdellinger/deep_learning_nanodegree_tv_script_generation_project/blob/master/requirements.txt)
