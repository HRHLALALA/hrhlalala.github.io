---
title: Trajectory Prediction Paper Literature Review
date: '2021-01-14'
layout: post
thumb_image: images/SE-GAN.png
toc: true
---


## Goal-GAN: Multimodal Trajectory Prediction Based on Goal Position Estimation
![](media/16105146218643/16105168936257.jpg)

### 1. Goal Module: 
* RGB image with $H \times W$ as module input
* U-Net as the encoder-decoder CNN network
    * Outputs a score map $\alpha = (\alpha_1, \alpha_2,\cdots, \alpha_n)$
    * Gumbel-Softmax Loss


### 2. Motion Encoder
* Simple LSTM block similar to Social GAN
* Aims to extract social features

### 3. Routing Module
* Consists of **an LSTM network**, **a visual soft attention network (ATT)**, and **an additional MLP layer that combines the attention map with the output of the LSTM** iteratively at each timestep.

### 4. Discriminator:
* 1 x LSTM for observation sequence
* 1 x LSTM for predicted sequence
* CNN for image patch centered around the current position at each time $t$
* 1 x LSTM for final output

### 5. Losses:
1. $L_2$ distance: 
$$\min_k ||Y - \hat{Y}^{k}||_2$$
2. Least Squares Generative Adversarial Network: 
$$L_{adv} = \frac{1}{2} E[D(X,Y) -1)^2 + \frac{1}{2}E[D(X,\hat{Y})^2]$$
3. Goal achievement losses: 
$$L_G = ||g-\hat{Y}^{t_{pred}}||$$
4. Cross-Entropy loss: 
$$L_{GCE} = -log(p_i)$$
5. Total Loss:
$$L = \lambda_{adv} L_{adv} + L_{L_2} + \alpha_G L_G + \lambda_{GCE} L_{GCE}$$


## Spatio-Temporal Graph Transformer Networks for Pedestrian Trajectory Prediction
![](media/16105146218643/16105207586767.jpg)
### 1. Temporal Transformer
$$
\newenvironment{rcases}
  {\left.\begin{aligned}}
  {\end{aligned}\right\rbrace}
  \begin{aligned}
\begin{rcases}
\textbf{Query:} \space  Q_i &= f_Q({h^i_j})\\
\textbf{Key:}K_i &= f_Q({h^i_j})\\
\textbf{Value:}V_i &= f_Q({h^i_j})\\
\end{rcases}
&\Longrightarrow 
Att(Q_i,K_i,V_i) = \frac{Softmax(Q_i K_{iT})}{\sqrt{d_k}} V_i\\
\\
&\Longrightarrow  MultiHead(Q_i,K_i,V_i) = f_O(Att(Q_i,K_i,V_i))
\end{aligned}
$$



### 2. Spatial Transformer
$$Attn(Q,K,V) = \frac{Q}{}$$

### 3. Spatio-Temporal Graph Transformer

{:color-style: style="background: black;"}
{:color-style: style="color: white;"}
{:text-style: style="font-weight: 800; text-decoration: underline;"}

|:             Here's an Inline Attribute Lists example                :||||
| ------- | ------------------ | -------------------- | ------------------ |
|:       :|:  <div style="color: red;"> &lt; Normal HTML Block > </div> :|||
| ^^      |   Red    {: .cls style="background: orange" }                |||
| ^^ IALs |   Green  {: #id style="background: green; color: white" }    |||
| ^^      |   Blue   {: style="background: blue; color: white" }         |||
| ^^      |   Black  {: color-style text-style }                         |||