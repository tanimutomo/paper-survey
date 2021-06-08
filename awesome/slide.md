---
marp: true

theme: gaia
size: 4:3
page_number: true
paginate: true
transition: "none"
style: | 
  h1 {
    font-size: 64px;
    text-align: center;
  }
  h2 { font-size: 42px; }
  h3 { font-size: 34px; }
  li { font-size: 26px; }
  p  { font-size: 26px; }
  img { width: 80%; }
---

<!-- _class: invert -->
# Awesome

Tomoki Tanimura (@tanimu)
d-hacks, Jin Nakazawa Lab, SFC, Keio University, M2

Created At: 2021/06/08

---

<!-- _class: invert -->
# Awesome Researches

- Dataset Distillation
- What’s Hidden in a Randomly Weighted Neural Network?
- ImageNet-Trained CNNs are biased towards texture; increasing shape bias improves accuracy and robustness
- Are Convolutional Neural Networks or Transformers more like human vision?

---

## How awesome are those researches?

- The point that no one address
- Everyone want to know that
- Sharp eyesight

---

# Dataset Distillation

- Model Distillation is to distill the knowledge of the large model to small one
- Dataset Distillation is to distill the knowledge of the large **Dataset** to small one

![](./asset/dataset_distillation_fig1.png)

---

## Dataset Distillation / Motivation

- How small can we compress the dataset knowledge?
- Distilled dataset can be used for continuous learning
- Can the model learn by the data sampled from incorrect distribution

![](./asset/dataset_distillation_intro_1.png)

---

## Dataset Distillation / Result

![](./asset/dataset_distillation_fig2.png)

---

# What’s Hidden in a Randomly Weighted Neural Network? (Hidden)

- Q. Does random network contains the subnetwork which can achieve good performance
- Find such subnetwork in large network with random weight
- Propose the efficient method to explore hidden subnetwork

---

## Hidden / Overview

![](./asset/hidden_fig1.png)

---

## Hidden / Related works

- "The Lottery Ticket Hypothesis"
  - Large random initialized NN has the subnetwork which has the potential to achieve the same performance as the entire network
- Some algorithms are proposed for finding WINiing-ticket effectively
- "WANNs (Weight Agnosstic Neural Network)"
  - Subnetwork of NN has same weight value can achieve almost same accuray as the trained one
  - But, this paper said we cannot  when random initialization 

---

## Hidden / Algorithm

- Set the score to each path
- Select the optimal path based on the score
- Update the scores with GD

![](./asset/hidden_fig2.png)

---

## Hidden / Result

![](./asset/hidden_table2.png)

---

# ImageNet-Trained CNNs are biased towards texture; increasing shape bias improves accuracy and robustness

- CNN see texture rather than shape

---

## Texture / Overview

 ![](./asset/texture_fig1.png)
 ![](./asset/texture_fig2.png)

---

## Texture / Compare CNN and Human

![](./asset/texture_fig4.png)

---

## Texture / Stylized dataset

![](./asset/texture_fig3.png)

---

## Texture / Performance of SIN

![](./asset/texture_table2.png)

---

# Are Convolutional Neural Networks or Transformers more like human vision?

- How about ViT?

---

## Transformer / Attention-based Networks

![](./asset/transformer_fig2.png)

---

## Transformer / Shape vs. Texture

- Finetune with effective data augmentation

![width:400px](./asset/texture_fig5.png) ![width:400px](./asset/texture_fig7.png)

---

# Summary

- Research what you wanna know
- Sharp eyesight
- ?

---