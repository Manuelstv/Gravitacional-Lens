# Astro-ML
Códigos implementados durante iniciação cientifica no if-ufrgs.



Detection of gravitational lensing systems using Machine Learning

Manuel Veras

Supervisor: Cristina Furlanetto

Universidade Federal do Rio Grande do Sul

In the near future, several large area photometric surveys will allow us to identify thousands
of strong gravitational lenses. Since simple visual inspection of the survey’s images would be
extremely laborious, it is a good idea to use machine learning techniques in order to classify
those images. In the recent years, several neural network architectures were developed in order
to increase efficiency. When it comes to image classification, the current state of the art are the
convolutional neural networks (CNNs).

In the field of astrophysics, several authors have developed CNNs to classify strong lensing
systems. However, one of the biggest challenges to increase efficiency in this architecture is
to provide a good training set, which consists of mocked lens images. For the purpose of im-
proving the training set it is a common practice to preprocess the mocked images. Following
that lead, in the following project, we aim at implementing a preprocessing algorithm to in-
vestigate if there is any improvement on the efficiency of the network to classify galaxy-scale
gravitational lenses.

The preprocessing algorithm consists of subtracting from an image a 180◦-rotated version
of itself, which we have called rotated-subtracted image. This is a purely geometrical technique,
which explores the approximate symmetry of elliptical galaxies (most common type of lenses)
and the asymmetry of the gravitational arcs to remove the light of the lenses, thus revealing
strong lensing features associated with the arcs. The advantage of this technique is that it
requires data from only one band, unlike other methods which require color information, i.e,
they require at least 2 bands.

To accomplish the goals of this project we have used the space-based images from the Strong
Gravitational Lens Finding Challenge (Metcalf et al. 2019) as our training and test sets. We
have chosen those given the potential application of the method on Euclid data.
In this work we have trained a CNN with two different training samples, one containing only
the original mocked images and the other containing those and also the corresponding rotated-
subtracted images. We will show the implemented algorithm and the preliminary results of the
comparison on the efficiency between the two methods on finding galaxy-scale lens systems.

![alt text](https://github.com/Manuelstv/Gravitacional-Lens/blob/main/poster%20sic2.png)

