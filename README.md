# Learning novel tasks from Visual Demonstrations

Can a VLM learn a novel visual task where the correct answer is not in the query text at all, but only possible to infer from the in-context examples?  For example, people will often ask a fully ambiguous question like "Is everything ok?" expecting the system to learn that the position of a certain object in the scene is sometimes good and sometimes bad, as in:

![SVAT Example](imgs/svat-example.png)

The model is expected to figure out that the green oval is the only thing changing in the image, and that there is some decision boundary for its location that distinguishes the YES and NO answers.  We call these tasks Spatial Visual Ambiguity Tasks (SVAT), and currently the decision boundary is restricted to either a horizontal or vertical line.  In this example, both the YES examples have the oval at the bottom of the image, while the NO examples have the oval near the top of the image, which should allow a well-trained VLM to infer that the correct answer is YES.

## Paper

The paper is available on arxiv at [https://arxiv.org/abs/2409.17080](https://arxiv.org/abs/2409.17080).

## Code for generating the SVAT dataset

This repository will contain the code used to create the datasets in our paper on learning from visual demonstrations.  Stay tuned!
