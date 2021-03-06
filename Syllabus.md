# Syllabus and materials
![Images generated using GanBreeder](Lessons/Media/GanBreederWide128.png)

(*Images created using [GanBreeder](https://ganbreeder.app/)*)

Here's all you needed for your first few weeks of creative AI and ML experiments, with supplementary materials to support further learning.

## Before the course
* [Prerequisites](Lessons/Prerequisites.md). Make sure you go through these before the course.

## Course structure
The lessons each include lecture slides and/or exercises. The exercises are in the form of Jupyter notebooks, and the links below open the notebooks in [Google Colab](https://colab.research.google.com/notebooks/intro.ipynb#), for which you need a Google account. [A note on Jupyter Notebooks, Colab, and other environments](Lessons/Jupyter_Colab_etc.md).



**Day 1:**
* Each student adds a slide in a shared Google Slides document: What's your background, what do you want to learn? This will help students to find teammates and teachers to customize the course contents
* Lecture: [Introduction and motivation](Lessons/LectureSlides/course_intro.pdf). Why one should rather co-create than compete with AI technology.
<!-- * Exercise: Processing images and audio as numbers. [[Open in Colab]](http://colab.research.google.com/github/PerttuHamalainen/MediaAI/blob/master/Code/Jupyter/ImagesAndAudio.ipynb) -->
* Exercise: Introduction to tensors, numpy and matplotlib, the basic tools you need for any scientific computing. [[Open in Colab]](http://colab.research.google.com/github/PerttuHamalainen/MediaAI/blob/master/Code/Jupyter/DataAndTensors.ipynb), [[Solutions]](http://colab.research.google.com/github/PerttuHamalainen/MediaAI/blob/master/Code/Jupyter/DataAndTensors_solutions.ipynb).

* Exercise: Training a very simple neural network using a [Kaggle](https://www.kaggle.com/) dataset of human height and weight. [[Open in Colab]](http://colab.research.google.com/github/PerttuHamalainen/MediaAI/blob/master/Code/Jupyter/PredictWeight.ipynb), [[Solutions]](http://colab.research.google.com/github/PerttuHamalainen/MediaAI/blob/master/Code/Jupyter/PredictWeight_solutions.ipynb)


**Day 2:**
* Lecture: [Neural networks, part 1](Lessons/LectureSlides/neural_networks_part1.pdf). Basics of neural networks, focusing on discriminative models like image classification.
* Exercise: Image classification, the bread-and-butter of neural networks. [[Open in Colab]](http://colab.research.google.com/github/PerttuHamalainen/MediaAI/blob/master/Code/Jupyter/MNIST.ipynb), [[Solutions]](http://colab.research.google.com/github/PerttuHamalainen/MediaAI/blob/master/Code/Jupyter/MNIST_solutions.ipynb)

* Optional exercise: Fooling the image classifier with adversarial images.  This is a bit more advanced topic, but included to demonstrate that discriminative models also have applications in generating images and visualizations. We will revisit the topic later. [[Open in Colab]](http://colab.research.google.com/github/PerttuHamalainen/MediaAI/blob/master/Code/Jupyter/AdversarialMNIST.ipynb). TODO: provide solutions.

* Optional exercise: Sound classification, to illustrate how processing audio can be done very similarly to images. [[Open in Colab]](http://colab.research.google.com/github/PerttuHamalainen/MediaAI/blob/master/Code/Jupyter/AudioMNIST.ipynb). TODO: Provide a solution to the exercise.  



**Day 3:**
* [Neural networks, part 2](Lessons/LectureSlides/neural_networks_part2.pdf). From discriminative to generative models like GANs. How to imbue computers with audiovisual imagination?
* Exercise: Generate and interpolate images using Google's BigGAN. [[Open in Colab]](http://colab.research.google.com/github/PerttuHamalainen/MediaAI/blob/master/Code/Jupyter/BigGAN%20test.ipynb), [[Solutions]](http://colab.research.google.com/github/PerttuHamalainen/MediaAI/blob/master/Code/Jupyter/BigGAN%20test_solutions.ipynb)


**Day 4:**
* [Neural networks, part 3](Lessons/LectureSlides/neural_networks_part3.pdf). Sequential problems like text prediction and generation.
* Exercise: Finetune OpenAI's GPT-2 text model with custom text. (TODO)
<!--* [Audio exercises, part 2](https://github.com/SopiMlab/DeepLearningWithAudio/blob/master/ICM_Audio/AudioExercises_part2/AudioClassification.md)-->

**Day 5:**
* [Optimization, part 1](Lessons/LectureSlides/optimization_part1.pdf). Pretty much all AI and ML is some form of (mathematical) optimization. We've already applied it when training neural networks; now it's the time to get a bit wider and deeper understanding. This first part deals with continuous-valued problems, focusing on two key algorithms: Adam and CMA-ES.
* Exercise: [Abstract Adversarial Image Optimization Using CMA-ES](http://colab.research.google.com/github/PerttuHamalainen/MediaAI/blob/master/Code/Jupyter/CMA-ES_Art.ipynb)
* Unity example (a Unity project folder that you can download and open in Unity): [Optimizing billiards trick shots in Unity](Code/Unity/IntelligentPool)

**Day 6:**
* [Optimization, part 2](Lessons/LectureSlides/optimization_part2.pdf). This part of the optimization lecture explains Deep Reinforcement Learning, building on the visual and geometric intuitions of CMA-ES.
* [Optimization, part 3](Lessons/LectureSlides/optimization_part3.pdf). Optimizing action sequences through Monte Carlo Tree Search, which provides an alternative to Deep RL, especially if there is a finite set of possible actions, e.g., gamepad buttons to press.  

The rest of the time is dedicated to project work that students can do either alone or in groups.

Note: The Jupyter exercises above use [Tensorflow](https://www.tensorflow.org/), which is the currently dominant deep learning library, although [PyTorch](https://pytorch.org/) is gaining in popularity. Those interested are encouraged to port the exercises to PyTorch!

## Colabs and Jupyter notebooks by others ##
These can provide starting points for your course projects. Note: the notebooks may take a while to run, but you can usually view or listen the pre-generated results without running the code. Disclaimer: I haven't had time to check that all of these run properly.

NOTE: if you get weird errors when running these on Colab, try adding ```%tensorflow_version 1.x``` to the beginning of the notebook, then select "Restart and run all" from the Runtime menu. Colab recently switched to Tensorflow 2 by default, but many of these notebooks precede the switch.

* [StyleGAN 2 finetuned with paintings](https://colab.research.google.com/drive/1cFKK0CBnev2BF8z9BOHxePk7E-f7TtUi#forceEdit=true&sandboxMode=true&scrollTo=jJRPjAU3Tn-K). Also see the [Reddit thread](https://www.reddit.com/r/MachineLearning/comments/bagnq6/p_stylegan_trained_on_paintings_512x512/?utm_content=title&utm_medium=post_embed&utm_name=44df278f7cb542cdb847cad34267b5ff&utm_source=embedly&utm_term=bagnq6)

* [NSynth for neural audio encoding, decoding, timestretching and interpolating](https://colab.research.google.com/drive/10wogut1V2ToGQZJcXH8StoMat6oWxoEu#scrollTo=0Fy4k_7SrnjH). N

* [GPT-2 text generation and finetuning the model with custom text](https://colab.research.google.com/drive/1VLG8e7YSEwypxU-noRNhsv5dW4NfTGce)

* [Neural style transfer for images](https://colab.research.google.com/github/log0/neural-style-painting/blob/master/TensorFlow%20Implementation%20of%20A%20Neural%20Algorithm%20of%20Artistic%20Style.ipynb)

* [A more complex BigGAN colab](https://colab.research.google.com/github/tensorflow/hub/blob/master/examples/colab/biggan_generation_with_tf_hub.ipynb)

* [A big Github repository of Jupyter notebooks for various topics, e.g., text, voice, visualization](https://github.com/firmai/awesome-google-colab). To open the notebooks in Colab, replace the https://github.com in the urls by https://colab.research.google.com/github.

* [12 Colab notebooks that matter](https://towardsdatascience.com/12-colab-notebooks-that-matter-e14ce1e3bdd0)



## Inspiration for further experiments
*a.k.a. Heroes of Creative AI and ML coding*

What to do with the skills and knowledge you gain on the course? Here are some people who are mixing AI, machine learning, art, and design with awesome results:

* http://otoro.net/ml/
* http://genekogan.com/
* http://quasimondo.com/
* http://zach.li/

## Supplementary material
* [ml5js](https://ml5js.org/) & [p5js](http://p5js.org/), the toolset that provides the fastest way to creative AI coding in a [browser-based editor](https://editor.p5js.org), without installing anything. Works even on mobile browsers! [This example](https://editor.p5js.org/AndreasRef/sketches/r1_w73FhQ) uses a deep neural network to track your nose and draw on the webcam view. [This one](https://editor.p5js.org/genekogan/sketches/Hk2Q4Sqe4) utilizes similar PoseNet tracking to control procedural audio synthesis.

* [Machine Learning for Artists (ml4a)](http://ml4a.github.io/), including many cool [demos](http://ml4a.github.io/demos/), many of them built using p5js and ml5js.  

* [Unity Machine Learning Agents](https://github.com/Unity-Technologies/ml-agents), a framework for using deep reinforcement learning for Unity. Includes code examples and blog posts.

* [Two Minute Papers](https://www.youtube.com/playlist?list=PLujxSBD-JXglGL3ERdDOhthD3jTlfudC2), a YouTube channel with short and accessible explanations of AI and deep learning research papers.

* [3Blue1Brown](https://www.youtube.com/channel/UCYO_jab_esuFRV4b17AJtAw), a YouTube channel with excellent visual explanations on math, including [neural networks](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi) and [linear algebra](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab).

* [Elements of AI](https://www.elementsofai.com/), an online course by University of Helsinki and Reaktor. Aalto students can also get 2 credits for this course. This is a course about the basic concepts, societal implications etc., no coding.

* [Game AI Book](http://gameaibook.org/) by Togelius and Yannakakis. PDF available.

* [Deep Learning book](https://www.deeplearningbook.org/) by Goodfellow et al. An excellent resource for digging deeper, for those that can handle some linear algebra, probability, and statistics. PDF available.


## Links
**The field is changing rapidly and we are constantly collecting new teaching material**

Follow the course's [Twitter feed](https://twitter.com/aaltomediaai) to stay updated.

[Back to course README](README.md)
