# Begin creating Deep Learning models

Following the advice of [Julia Evans](https://jvns.ca/blog/2016/05/22/how-do-you-write-blog-posts/), I'm going to write about things that I wish I knew a year ago.
Machine Learning research sometimes feels like an activity reserved for the intellectually superior, while us mere mortals enjoy their trimmings when they publish and the open-source community implements it.

!["Please, can I have an open-source implementation?"](https://github.com/scottire/scottire.github.io/blob/master/images/1_jnnJQ2XJbyZ5zgf95onIJw.jpeg?raw=true)

## You don't need a PhD

This myth was completely debunked for me when I took the fast.ai course, [Practical Deep Learning for Coders, v3](https://course.fast.ai/). So my first tip, do it. Also, [this post by Rachel Thomas](https://www.fast.ai/2018/08/27/grad-school/) gives some great advice to those thinking about grad school.

If some of the stuff below seems like gibberish, fast.ai is a good place to go.

## Tips for people wanting to begin creating / improving deep learning models.

Find a dataset that interests you.
[Here](https://towardsdatascience.com/top-sources-for-machine-learning-datasets-bb6d0dc3378b)'s a good post about where to find it. 
Try not to get analysis paralysis, just choose one. You're not married to the dataset you choose, but get to know it.

[Here](https://www.kaggle.com/learn/overview) are plenty of resources to learn to visualize and analyze a dataset.

## Use Google Colab

If you want free access to a GPU, [here you go](http://colab.research.google.com/).
[If you want to know why or setting up a GPU is becoming frustrating.](https://towardsdatascience.com/getting-started-with-google-colab-f2fff97f594c)

## Get 100% accuracy on one instance/batch of your data

Rather than wasting your time loading all of the data each time you want to check for bugs, create a _tiny dataset_ with just one instance of your dataset and overfit it with a very simple model.

##  Get 100% accuracy on around 10% of your data

Once you can overfit your model on one instance, begin using more of your data and try to overfit it by adding more layers. Don't use any regularization for the moment (e.g., Dropout, L1/ L2 regularization), this is another sanity preserving tip so you know that your model is learning.

##  Add all of your training data

Once you add all of your data, if training is taking too long, leave it aside as an experiment and continue your work on the 10% of data. If you're overfitting when you add more layers and all of your data, here's five steps to reduce overfitting.

![Source: fast.ai](https://github.com/scottire/scottire.github.io/blob/master/images/avoid_overfitting.jpeg?raw=true)

And that's it for today, those tips are some of the valuable gems that I wish I found out sooner.
If have any feedback, [here's me on Twitter](https://twitter.com/_ScottCondron).

_Thanks for reading_
