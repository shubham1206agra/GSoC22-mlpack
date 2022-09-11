
![GSoC mlpack image](./assets/gsoc-mlpack.png)

**Organisation: [mlpack](https://github.com/mlpack)**

**Project: [Ready to use Models](https://summerofcode.withgoogle.com/programs/2022/projects/ujTRUswo)**

**Mentors: [Ryan Curtin](https://github.com/rcurtin), [Jeffin Sam](https://github.com/jeffin143) and [Kartik Dutt](https://github.com/kartikdutt18)**

## Abstract

I was selected for google summer of code 2022 to work with mlpack on the project `Ready to use models in mlpack`. Mlpack is an intuitive, fast, and flexible C++ machine learning library with bindings to other languages. In recent years computer vision has taken many turns and at this point, it is at a mature stage that when you need to use say a classification model you don't need to construct the complete architecture on your own, you can just write a single line of code and it creates the complete pretrained model for you which is what I did and added multiple models with pretrained weights on imagenet. 

## Goal

The aim is to implement various pre-trained models ranging from very basic AlexNet to super complex models, including implementing different layers such as depthwise separable convolutions, inception layers, and residual layers. This project would fall under the idea: Ready to use models in mlpack, the pre-trained models will fall under the models repository, and layers will fall under the mlpack repository as a layer inside the artificial neural network (ANN) codebase.


## Results

All the models that I proposed with pretrained weights with a lot of configuration are now available in the mlpack codebase. On the way, we faced and discovered small issues or implementation bugs which we corrected but we still face some issues with the parallelization of ANN layers and requires GPU support in the future to speed up, but I would like to thank Kartik because yes the format I choose for writing this is originally his and yes this is 100% inspired by his with little tweaks of mine. 

## g++ Contributions.cpp -o Contributions

I have divided my contributions according to the repositories and PR having this 👍 symbol in front of them was the core part of my projects others were mostly the ones that I picked up on the way but weren't mentioned in my project.

### [mlpack/models](https://github.com/mlpack/models)

- [AlexNet Implementation](https://github.com/mlpack/models/pull/76) 👍
- [SqueezeNet Implentation](https://github.com/mlpack/models/pull/77) 👍
- [VGG Implementation](https://github.com/mlpack/models/pull/78) 👍
- [Xception Implementation](https://github.com/mlpack/models/pull/79) 👍
- [Catch Update](https://github.com/mlpack/models/pull/80)

### [mlpack/mlpack](https://github.com/mlpack/mlpack)

- [AddMerge Layer Implementation](https://github.com/mlpack/mlpack/pull/3224) 👍
- [Correction in ANN layers](https://github.com/mlpack/mlpack/pull/3229)
- [Batch Norm Implementation](https://github.com/mlpack/mlpack/pull/3231) 👍
- [FFN Hotfix](https://github.com/mlpack/mlpack/pull/3232)
- [Adaptive Pooling Hotfix](https://github.com/mlpack/mlpack/pull/3234)
- [Convolution Hotfix](https://github.com/mlpack/mlpack/pull/3236)
- [Parallelize ANN with OpenMP](https://github.com/mlpack/mlpack/pull/3240) 👍
- [Identity Layer implementation](https://github.com/mlpack/mlpack/pull/3242) 👍
- [Bias Boolean in Convolution layer](https://github.com/mlpack/mlpack/pull/3244) 👍
- [Grouped Convolution](https://github.com/mlpack/mlpack/pull/3247) 👍
- [Serialization Hotfix](https://github.com/mlpack/mlpack/pull/3252)
- [Make Install BugFix](https://github.com/mlpack/mlpack/pull/3257)

### [mlpack-weight-converter](https://github.com/shubham1206agra/mlpack-weight-converter)

This repository was used to port weights for all the models from Pytorch using [shubham1206agra](https://github.com/shubham1206agra) / **[pretrained-models.pytorch](https://github.com/shubham1206agra/pretrained-models.pytorch)** in torch hub.

## Final Thoughts

I loved the time I spent with mlpack and would like to thanks all my mentors  for guiding me with the best practices and helping me out whenever I was stuck. I would keep contributing to the project and the community as a whole with the things I have learned and would continue to learn.

## Ways to reach me

<p align="center">
  <a href="mailto:shubham.agra1206@gmail.com?subject = Hello from your GitHub README&body = Message"><img src="./assets/gmail.svg" height="80px" width="80px" alt="Gmail" ></a>
  <a href="https://www.linkedin.com/in/shubham-agrawal-113802180/"><img src="./assets/linkedIn.svg" height="80px" width="80px" alt="LinkedIn"></a>
</p>
