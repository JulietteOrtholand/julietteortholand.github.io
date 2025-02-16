---
layout: page
title: Pyraug
description: A python library to perform data augmentation with VAEs
img: assets/img/pyraug_project/logo_pyraug_2.jpeg
github: https://github.com/clementchadebec/pyraug
documentation: https://pyraug.readthedocs.io/en/latest/
licence: https://opensource.org/licenses/Apache-2.0
stars: https://github.com/clementchadebec/pyraug/stargazers
pypi_package: https://pypi.org/project/pyraug/
arxiv: https://arxiv.org/abs/2105.00026
importance: 1
category: old

bibliography: 2018-12-22-distill.bib
---

<p style="margin-bottom: 2em">
</p>


### Why data augmentation ?

Even <d-cite key="ucar_bridging_2019"></d-cite>
though always larger data sets are now available, the lack of labeled data remains a tremendous issue in many fields of application. Among others, a good example is healthcare where practitioners have to deal most of the time with (very) low sample sizes (think of small patient cohorts) along with very high dimensional data (think of neuroimaging data that are 3D volumes with millions of voxels). Unfortunately, this leads to a very poor representation of a given population and makes classical statistical analyses unreliable. Meanwhile, the remarkable performance of algorithms heavily relying on the deep learning framework has made them extremely attractive and very popular. However, such results are strongly conditioned by the number of training samples since such models usually need to be trained on huge data sets to prevent over-fitting or to give statistically meaningful results. A way to address such issues is to perform Data Augmentation (DA) which consists in creating synthetic samples to enrich an initial data set and allow machine learning algorithm to better generalize on unseen data. For instance, the easiest way to do this on images is to apply simple transformations such as the addition of Gaussian noise, cropping or padding, and assign the label of the initial image to the created ones.

### Limitations of classic DA

While such augmentation techniques have revealed very useful, they remain strongly data dependent and limited. Some transformations may indeed be uninformative or even induce bias. For instance, think of a digit representing a 6 which gives a 9 when rotated. While assessing the relevance of augmented data may be quite straightforward for simple data sets, it reveals very challenging for complex data and may require the intervention of an _expert_ assessing the degree of relevance of the proposed transformations.

### Generative models: A new hope

The recent rise in performance of generative models such as GAN or VAE has made them very attractive models to perform DA. However, the main limitation to a wider use of these models is that they most of the time produce blurry and fuzzy samples. This undesirable effect is even more emphasized when they are trained with a small number of samples which makes them very hard to use in practice to perform DA in the high dimensional (very) low sample size (HDLSS) setting.

**This is why Pyraug was born!**
