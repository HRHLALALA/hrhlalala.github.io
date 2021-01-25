---
title: Trajectory Forecasts in Unknown Environments Conditioned on Grid-Based Plans (Literacture Review)
date: '2021-01-25'
layout: post
thumb_image: images/P2TIRL.jpg
toc: true
---

## Introduction
> This paper proposes P2TIRL that uses a maximum entropy inverse reinforcement learning policy to infer goal and trajectory plan over a discrete grid. P2TRL assigns rewards to future goals that are learned by the training policy which is slow and computationally expensive.


Authors:
* Nachiket Deo
* Mohan M. Trivedi

## Maximum Entropy Inverse Reinforcement Learning for Path Forecasting
### Markov Decision Process
$$M = \{S,A,T,r\}$$
* $S$: the state space consisting of cells in a 2-D grid deﬁned over the scene.
* $A$: action space consisting of 4 discrete actions: {up,down,left,right}
* $T$: state transition function where $S_{n-1} \times A \rightarrow S_n$
* $r$: reward function mapping each state to a real value less or equal to 0

### Probability Formation
$$P(\tau) = \frac{1}{Z} \exp{(r(\tau))} = \frac{1}{Z} \exp({\sum_{i=1}^N r(s_i)})$$
* $Z$ is the normalising constant for $\sum{P} =1$
* $r_\theta(s)$ is the reward function parameterised by $\theta$

### Object
The objective is to learn a reward function that maximises the log likelihood of observing a training set of demonstrations $\tau \in T = \{\tau_1,\tau_2, \cdots, \tau_n\}$
$$\arg \max_\theta L_\theta = \arg \max_\theta \sum_{\tau \in T}\log(P(\tau))$$

This can be solved using 
$$
    \frac{\delta L_\theta}{\delta \theta} = \sum_{\tau \in T}(D_\tau - D_\theta) \frac{\delta r_\theta}{\delta \theta}
$$
* $D$ is the state visitation algorithm
    1. calculate $\pi_\theta(a|s)$: the probability of taking action $a$ given state $s$
![-w539](media/16114838146872/16115004658300.jpg)
    1. calculate $D$ using $\pi_\theta$
![-w544](media/16114838146872/16115004432641.jpg)


* 


## Model Architecture
![-w1121](media/16114838146872/16115006830592.jpg)
### Reward Learning
![-w530](media/16114838146872/16115016400122.jpg)

**Path reward**:
    $$r_{p_\theta} = CNN_p(\phi_I,\phi_M)$$

**Goal reward**
    $$r_{g_\theta} = CNN_g(\phi_I,\phi_M)$$ 
    
* $\phi _I = CNN_{feat}(I)$
* $\phi _M = [\|v\|, \Delta \theta, r]$ where 
    * $\|v\|$: speed
    * $\Delta \theta$: angular deviation between a cell location and the instantaneous direction of the agents' motion.
    * $r$: distance 
* $CNN_{feat}(I)$ is pretrained on ISPRS Potsdam dataset 

### Approximate Value Iteration with inferred goals

![-w535](media/16114838146872/16115030123633.jpg)
* Main difference:
    1. Do not hold the $V(s_{goal})$ ﬁxed at 0 to enforce goal directed behavior.
![-w541](media/16114838146872/16115030268453.jpg)


### Trajectory Generator
**Motion encoder**: $$h_{m_t} = GRU(h_{m_{t-1}}, e_x(X_t))$$
* $e_x(\cdot)$ is a fully connected embedding layer for the track co-ordinates.

**Plan encoder**: 
![-w544](media/16114838146872/16115027395288.jpg)

$$
    h_{s_n}^{(i)} = BiGRU(h_{s_n}^{(i-1)},h_{s_n}^{(i+1)},\phi_s(s_n))
$$
* two inputs concatenated as the input:
    * position coordinate
    * scene patch

**Attention based Encoder**
$$h_{dec_t}^{(i)} = GRU_{dec}(h_{t-1}^{(i)}, Attn(h_{t-1}^{(i)},h_{S_{1:N}}^{(i)}))$$
* $h_0$: final hidden state from motion encoder
* Attention mechanism: soft attention
    * Pay attention to a specific state 
* Decoder: $GRU$


## Results
![-w474](media/16114838146872/16115031805533.jpg)
