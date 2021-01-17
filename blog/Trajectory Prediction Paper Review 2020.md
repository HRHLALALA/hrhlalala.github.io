---
title: Trajectory Prediction Paper Literature Review
date: '2021-01-14'
layout: post
thumb_image: images/SE-GAN.png
toc: true
---

| Paper                                                                                                                                                                                                                      | Year | Conference | Keywords                                                                                                                             | Paper Link                                                                                                                                                                                   | Code                                                        |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---- | ---------- | ------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------- |
| [CoL-GAN: Plausible and Collision-Less Trajectory Prediction by Attention-Based GAN](#col-gan-plausible-and-collision-less-trajectory-prediction-by-attention-based-gan)                                                 | 2020 | IEEE       | CNN-Based Discriminator; Attention Module in Decoder; Relative position and speed as Attention Input                                 | [link](https://ieeexplore.ieee.org/ielx7/6287639/8948470/09063432.pdf)                                                                                                                       |                                                             |
| [DAG-Net: Double Attentive Graph Neural Network for Trajectory Forecasting](#dag-net-double-attentive-graph-neural-network-for-trajectory-forecasting)                                                                   | 2020 | ICPR       | Recurrent VAE;                                                                                                                       | [link](https://arxiv.org/pdf/2005.12661.pdf)                                                                                                                                                 | [link](https://github.com/alexmonti19/dagnet)               |
| [Dynamic and Static Context-aware LSTM for Multi-agent Motion Prediction](#dynamic-and-static-context-aware-lstm-for-multi-agent-motion-prediction)                                                                      | 2020 | ECCV       | Individual Context Module; Social Aware Context Module; Sematntic Guidence; Temporal Correlation Coefficient                         | [link](https://arxiv.org/pdf/2008.00777.pdf)                                                                                                                                                 |                                                             |
| [EvolveGraph: Multi-Agent Trajectory Prediction with Dynamic Relational Reasoning](#evolvegraph-multi-agent-trajectory-prediction-with-dynamic-relational-reasoning)                                                     | 2020 | NeurIPS    | Graph Learning; Static and Dynamic Interaction;GAT-like method                                                                       | [link](https://arxiv.org/pdf/2003.13924.pdf)                                                                                                                                                 |                                                             |
| [Goal-driven Long-Term Trajectory Prediction ](#goal-driven-long-term-trajectory-prediction)                                                                                                                             | 2021 | WACV       | Goal Channel; Controller sub-network                                                                                                 | [link](https://openaccess.thecvf.com/content/WACV2021/papers/Tran_Goal-Driven_Long-Term_Trajectory_Prediction_WACV_2021_paper.pdf)                                                           |                                                             |
| [Goal-GAN:Multimodal Trajectory Prediction Based on Goal Position Estimation](#goal-gan-multimodal-trajectory-prediction-based-on-goal-position-estimation)                                                              | 2020 | ACCV       | Goal Estimation; Routing Module; Gumbel Sampling; Attn Decoder; GAN;                                                                 | [link](https://arxiv.org/pdf/2010.01114.pdf)                                                                                                                                                 | [link](https://github.com/dendorferpatrick/GoalGAN)         |
| [GraphTCN: Spatio-Temporal Interaction Modeling for Human Trajectory Prediction](#graphtcn-spatio-temporal-interaction-modeling-for-human-trajectory-prediction)                                                         | 2021 | WACV       | Edge feature based graph attention network(EFGAT); Temporal convolutional network(TCN);                                              | [link](https://openaccess.thecvf.com/content/WACV2021/papers/Wang_GraphTCN_Spatio-Temporal_Interaction_Modeling_for_Human_Trajectory_Prediction_WACV_2021_paper.pdf)                         |                                                             |
| [How Can I See My Future? FvTraj: Using First-person View for Pedestrian Trajectory Prediction](#how-can-i-see-my-future-fvtraj-using-first-person-view-for-pedestrian-trajectory-prediction)                            | 2020 | ECCV       | Attention Module; Simulated first-person view image                                                                                  | [link](http://graphics.cs.uh.edu/wp-content/papers/2020/2020-ECCV-PedestrianTrajPrediction.pdf)                                                                                              |                                                             |
| [Human Trajectory Forecasting in Crowds: A Deep Learning Perspective](#human-trajectory-forecasting-in-crowds-a-deep-learning-perspective)                                                                               | 2020 | ArXiv      | Literature Review; Non-grid Based &  Grid-based;                                                                                    | [link](https://arxiv.org/pdf/2007.03639.pdf)                                                                                                                                                 |                                                             |
| [It is not the Journey but the Destination- Endpoint Conditioned Trajectory Prediction](#it-is-not-the-journey-but-the-destination-endpoint-conditioned-trajectory-prediction)                                           | 2020 | ECCV       | Goal-based method; VAE; KL Divergence Loss; Average Endpoint Los, Average Trajctory Loss; Non-Local Social Pooling; Truncation trick | [link](https://arxiv.org/pdf/2004.02025.pdf)                                                                                                                                                 |                                                             |
| [Recursive Social Behavior Graph for Trajectory Prediction ](#recursive-social-behavior-graph-for-trajectory-prediction)                                                                                                 | 2020 | CVPR       | CNN for Patch Image Input; BiLSTM; GCN; Handcraft Group Annotation; Exponential Loss                                                 | [link](https://openaccess.thecvf.com/content_CVPR_2020/papers/Sun_Recursive_Social_Behavior_Graph_for_Trajectory_Prediction_CVPR_2020_paper.pdf)                                             |                                                             |
| [Self-Growing Spatial Graph Networks for Pedestrian Trajectory Prediction ](#self-growing-spatial-graph-networks-for-pedestrian-trajectory-prediction)                                                                   | 2020 | WACV       | Spatial Graphic Network; Multiple Stacked GRU; motion features;                                                                      | [link](https://openaccess.thecvf.com/content_WACV_2020/papers/Haddad_Self-Growing_Spatial_Graph_Networks_for_Pedestrian_Trajectory_Prediction_WACV_2020_paper.pdf)                           |                                                             |
| [SILA: An Incremental Learning Approach for Pedestrian TrajectoryPrediction](#sila-an-incremental-learning-approach-for-pedestrian-trajectoryprediction)                                                                 | 2020 | CVPR       | Similarty -based Icremental Learning Algorithm; Speed Improve;                                                                       | [link](https://openaccess.thecvf.com/content_CVPRW_2020/papers/w66/Habibi_SILA_An_Incremental_Learning_Approach_for_Pedestrian_Trajectory_Prediction_CVPRW_2020_paper.pdf)                   |                                                             |
| [SMART: Simultaneous Multi-Agent Recurrent Trajectory Prediction](#smart-simultaneous-multi-agent-recurrent-trajectory-prediction)                                                                                       | 2020 | ECCV       | ConvLSTM;CVAEs; O(1)                                                                                                                 | [link](https://arxiv.org/pdf/2007.13078.pdf)                                                                                                                                                 |                                                             |
| [Social NCE: Contrastive Learning of Socially-aware Motion Representations](#social-nce-contrastive-learning-of-socially-aware-motion-representations)                                                                   | 2020 | NeurIPS    |  Contrastive Represent Learning; InfoNCE Loss; Contrastive Sampling                                                                  | [link](https://arxiv.org/pdf/2012.11717.pdf)                                                                                                                                                 | [link](https://github.com/vita-epfl/social-nce)             |
| [Social-STGCNN: A Social Spatio-Temporal Graph Convolutional Neural Network for Human Trajectory Prediction](#social-stgcnn-a-social-spatio-temporal-graph-convolutional-neural-network-for-human-trajectory-prediction) | 2020 | CVPR       | GCNN;                                                                                                                                | [link](https://openaccess.thecvf.com/content_CVPR_2020/papers/Mohamed_Social-STGCNN_A_Social_Spatio-Temporal_Graph_Convolutional_Neural_Network_for_Human_CVPR_2020_paper.pdf)               | [link](https://github.com/abduallahmohamed/Social-STGCNN)   |
| [Social-WaGDAT: Interaction-aware Trajectory Prediction via Wasserstein Graph Double-Attention Network](#social-wagdat-interaction-aware-trajectory-prediction-via-wasserstein-graph-double-attention-network)           | 2020 | ArXiv      | Two GAT system; Kinematic Constraint;Wasserstein generative learning                                                                 | [link](https://arxiv.org/pdf/2002.06241.pdf)                                                                                                                                                 |                                                             |
| [Spatio-Temporal Graph Transformer Networks for Pedestrian Trajectory Prediction](#spatio-temporal-graph-transformer-networks-for-pedestrian-trajectory-prediction)                                                      | 2020 | ECCV       | Transformer Network; TGConv; 2-encoder structure; Graph Memory                                                                       | [link](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123570494.pdf)                                                                                                               | [link](https://github.com/Majiker/STAR)                     |
| [The Garden of Forking Paths: Towards Multi-Future Trajectory Prediction](#the-garden-of-forking-paths-towards-multi-future-trajectory-prediction)                                                                       | 2020 | CVPR       | multi-scale location encodings; convolutional RNNs over graphs                                                                       | [link](https://openaccess.thecvf.com/content_CVPR_2020/papers/Liang_The_Garden_of_Forking_Paths_Towards_Multi-Future_Trajectory_Prediction_CVPR_2020_paper.pdf)                              |                                                             |
| [Trajectron++: Dynamically-Feasible Trajectory Forecasting With Heterogeneous Data](#trajectron-dynamically-feasible-trajectory-forecasting-with-heterogeneous-data)                                                     | 2020 | ECCV       |                                                                                                                                      | [link](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123630664.pdf)                                                                                                               | [link](https://github.com/StanfordASL/Trajectron-plus-plus) |
| [Multiple Futures Prediction](#multiple-futures-prediction)                                                                                                                                                              | 2019 | NeurIPS    |                                                                                                                                      | [link](http://papers.nips.cc/paper/9676-multiple-futures-prediction.pdf)                                                                                                                     |                                                             |
| [STGAT: Modeling Spatial-Temporal Interactions for Human Trajectory Prediction](#stgat-modeling-spatial-temporal-interactions-for-human-trajectory-prediction)                                                           | 2019 | ICCV       | GAT; Spatio-temporal                                                                                                                 | [link](http://openaccess.thecvf.com/content_ICCV_2019/papers/Huang_STGAT_Modeling_Spatial-Temporal_Interactions_for_Human_Trajectory_Prediction_ICCV_2019_paper.pdf)                         |                                                             |
| [Social and Scene-Aware Trajectory Prediction in Crowded Spaces](#social-and-scene-aware-trajectory-prediction-in-crowded-spaces)                                                                                        | 2019 | ICCV       | Schematic segmented Scenes                                                                                                           | [link](https://arxiv.org/pdf/1909.08840.pdf)                                                                                                                                                 | [link](https://github.com/Oghma/sns-lstm/)                  |
| [Trajectory Prediction by Coupling Scene-LSTM with Human Movement LSTM ](#trajectory-prediction-by-coupling-scene-lstm-with-human-movement-lstm)                                                                         | 2019 | ISVC       | Grid-based Modelling                                                                                                                 | [link](https://arxiv.org/pdf/1908.08908.pdf)                                                                                                                                                 |                                                             |
| [Scene Compliant Trajectory Forecast with Agent-Centric Spatio-Temporal Grids ](#scene-compliant-trajectory-forecast-with-agent-centric-spatio-temporal-grids)                                                           | 2019 | ArXiv      | Grid representation for scene and trajectory; ConvCNN; Scene Heatmap  Output;                                                        | [link](https://arxiv.org/pdf/1909.07507.pdf)                                                                                                                                                 |                                                             |
| [trajectory Prediction of Mobile Construction Resources Toward Pro-active Struck-by Hazard Detection](#trajectory-prediction-of-mobile-construction-resources-toward-pro-active-struck-by-hazard-detection)              | 2019 | ISARC      | Hyperparamter Tunning                                                                                                                | [link](https://www.iaarc.org/publications/fulltext/ISARC_2019_Paper_201.pdf)                                                                                                                 |                                                             |
| [Learning to Infer Relations for Future Trajectory Forecast ](#learning-to-infer-relations-for-future-trajectory-forecast)                                                                                               | 2019 | CVPR       | 2D+3D for spatial temporal features; Heatmap Generation; Monte Carlo dropout                                                         | [link](https://openaccess.thecvf.com/content_CVPRW_2019/papers/Precognition/Choi_Learning_to_Infer_Relations_for_Future_Trajectory_Forecast_CVPRW_2019_paper.pdf)                            |                                                             |
| [Looking to Relations for Future Trajectory Forecast ](#looking-to-relations-for-future-trajectory-forecast)                                                                                                             | 2019 | ICCV       | Relational Model;                                                                                                                    | [link](https://openaccess.thecvf.com/content_ICCV_2019/papers/Choi_Looking_to_Relations_for_Future_Trajectory_Forecast_ICCV_2019_paper.pdf)                                                  |                                                             |
| [Multi-Agent Tensor Fusion for Contextual Trajectory Prediction](#multi-agent-tensor-fusion-for-contextual-trajectory-prediction)                                                                                        | 2019 | CVPR       | Spatial Fusion; GAN;                                                                                                                 | [link](https://openaccess.thecvf.com/content_CVPR_2019/papers/Zhao_Multi-Agent_Tensor_Fusion_for_Contextual_Trajectory_Prediction_CVPR_2019_paper.pdf)                                       |                                                             |
| [SR-LSTM: State Refinement for LSTM towards Pedestrian Trajectory Prediction ](#sr-lstm-state-refinement-for-lstm-towards-pedestrian-trajectory-prediction)                                                              | 2019 | CVPR       | Soft Attention;  Social Intraction; Information filter                                                                               | [link](https://openaccess.thecvf.com/content_CVPR_2019/papers/Zhang_SR-LSTM_State_Refinement_for_LSTM_Towards_Pedestrian_Trajectory_Prediction_CVPR_2019_paper.pdf)                          | [link](https://github.com/zhangpur/SR-LSTM)                 |
| [Social Ways: Learning Multi-Modal Distributions of Pedestrian Trajectories With GANs](#social-ways-learning-multi-modal-distributions-of-pedestrian-trajectories-with-gans)                                             | 2019 | CVPR       | Info GAN                                                                                                                             | [link](http://openaccess.thecvf.com/content_CVPRW_2019/papers/Precognition/Amirian_Social_Ways_Learning_Multi-Modal_Distributions_of_Pedestrian_Trajectories_With_GANs_CVPRW_2019_paper.pdf) | [link](https://github.com/amiryanj/socialways)              |
                                                                            
## Goal-GAN: Multimodal Trajectory Prediction Based on Goal Position Estimation
![](media/16105146218643/16105168936257.jpg)
This paper proposes Goal-GAN, a two-stage end-to-end trainable trajectory prediction method inspired by human navigation, which separates the prediction task into goal position estimation and routing. It designs a novel architecture that explicitly estimates an interpretable probability distribution of future goal positions and allows us to sample from it.

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
![-w758](media/16105146218643/16105207586767.jpg)
This paper presents Predicted Endpoint Conditioned Network (PECNet) for ﬂexible human trajectory prediction. PECNet infers distant trajectory endpoints to assist in long-range multi-modal trajectory prediction. A novel nonlocal social pooling layer enables PECNet to infer diverse yet socially compliant trajectories. Additionally, we present a simple “truncation-trick” for improving diversity and multi-modal trajectory prediction performance.

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

### 1. Endpoint VAE

* Definition:
    * past histories:  $\tau^k_p = \{(x,y)\}_{i=1}^{t_f}$ for pedestrian $p_k$ 
    * socially compliant future trajectories $\tau^k_f = \{(x,y)\}_{i=t_p + 1}^{t_p+t_f}$ for pedestrian $p_k$.
    * finally: $\hat{\mathcal{G}_k}, \mathcal{G}_k = \{(x,y)\}\rvert  _{t_p+t_f} $.
    

* Detail:

$$
  \newenvironment{rcases}
    {\left.\begin{aligned}}
    {\end{aligned}\right\rbrace}
    \begin{aligned}
  \begin{rcases}
  \space  \mathbf{E}_{past}(\tau_i)\\
  \textbf{Key:}\space\mathbf{E}_{end}(\mathcal{G}_i)\\
  \end{rcases}
  &\xrightarrow{\mathbf{E}_{latent}}
  (\mu,\sigma)\Rightarrow N(\mu,\sigma^2) \sim Z \\\\
  \Longrightarrow
  \begin{rcases}
  Z\\
  \mathbf{E}_{past}(\tau_i)
  \end{rcases}
  &\xrightarrow{\mathbf{D}_{latent}} \hat{\mathcal{G}}_i
  \end{aligned}
  $$


### 2. Endpoint conditioned Trajectory Prediction
Social Pooling Matrix:
![-w1284](media/16105146218643/16107326363430.jpg)
![-w1207](media/16105146218643/16107332023249.jpg)


### 3. Loss
![-w1125](media/16105146218643/16107329252827.jpg)
* KL divergence term is used for training the Variational Autoencoder
* the Average endpoint Loss (AEL) trains $E_{end}$, $E_{past}$, $E_{latent}$ and $D_{latent}$
* Average Trajectory Loss (ATL) trains the entire module together.


## EvolveGraph: Multi-Agent Trajectory Prediction with Dynamic Relational Reasoning
![-w949](media/16105146218643/16108926207575.jpg)
The main contributions of this paper are summarized as:

* It proposes a generic trajectory forecasting framework with explicit interaction modelling via a latent graph among multiple heterogeneous, interactive agents. Both trajectory information and context information (e.g. scene images, semantic maps, point cloud density maps) can be incorporated into the system.

* It proposes a dynamic mechanism to evolve the underlying interaction graph adaptively along time, which captures the dynamics of interaction patterns among multiple agents. We also introduce a double-stage training pipeline which not only improves training efﬁciency and accelerates convergence, but also enhances model performance in terms of prediction accuracy.

* The proposed framework is designed to capture the uncertainty and multi-modality of future trajectories in nature from multiple aspects.

* The proposed framework is validated on both synthetic simulations and trajectory forecasting benchmarks in different areas. Our EvolveGraph achieves the state-of-the-art performance consistently.

### 1. Static interact on graph learning
![-w610](media/16105146218643/16108970156443.jpg)

* **Observation Graph** aims to extract feature embeddings from raw observations, which consists of N agent nodes and one context node. Agent nodes are bidirectionally connected to each other, and the context node only has outgoing edges to each agent node. Each agent node has two types of attributes: self-attribute and social-attribute. The former only contains the node’s own state information, while the latter only contains other nodes’ state information.

* **Interaction Graph** is presented by different edge type. No edge between a pair of nodes means that the two nodes have no relation. The interaction graph represents interaction patterns with a distribution of edge types for each edge, which is built on top of the observation graph.

 
* **Encoding process** is to infer a latent interaction graph from the observation graph, which is essentially a multi-class edge classification task.

* **Recurrent Decoder**is applied to the interaction graph and observation graph to approximate the distribution of future trajectories.

### 2. Dynamic interaction graph
In many situations, the interaction patterns recognized from the past time steps are likely not static in the future. Moreover, many interaction systems have multi-modal properties in nature. Different modalities afterwards are likely to result in different interaction patterns and outcomes. Therefore, we designed a dynamic evolving process of the interaction patterns.

### 3. Uncertainty and Multi-modality
1. Gaussian Mixture distribution in decoder
2. Different sampled trajectories will lead to different interaction graph evolution.
3. Variety loss

### 4. Loss
![-w1191](media/16105146218643/16108975158902.jpg)


## Social-WaGDAT: Interaction-aware Trajectory Prediction via Wasserstein Graph Double-Attention Network
![-w840](media/16105146218643/16107019503809.jpg)
This paper proposes a generic generative neural system (called Social-WaGDAT) for multi-agent trajectory prediction, which makes a step forward to explicit interaction modelling by incorporating relational inductive biases with a dynamic graph representation and leverages both trajectory and scene context information. We also employ an efficient kinematic constraint layer applied to vehicle trajectory prediction which not only ensures physical feasibility but also enhances model performance.

### 1. Feature Extraction
* **State MLP** embeds the position
* **Relation MLP** embeds the relative information between each pair of agents
    * The distance and relative angle (in a 2D polar coordinate)
    * The differences between the positions of the two agents along two axes
* **Context CNN** extracts spatial features for each agent from a local occupancy density map $(H \times W \times 1)$ as well as heuristic features from a local velocity ﬁeld $(H \times W \times 2)$ centered on the corresponding agent.


### 2. Encoder with Graphic Double Attention(GDAT)
* History Graph & Future Graph
    * the state features and context features are concatenated to be the node attributes
    * the relation features are used as edge attributes.
    * generated and processed in a similar fashion but with different time stamps.
    * The number of nodes (agents) in a graph is assumed to be ﬁxed, but the edges are eliminated if the spatial distance between two nodes is larger than a threshold.
* Topological Attention Layer
    * the agents with similar node attributes to the objective agent or with small spatial distance should be paid more attention to. 
* Temporal Attention Layer
    * Input is the output of the topological ¯V attention layer
    
### 2. Decoder with Kinematic Constraint
$$
\begin{cases} 
    \dot{x} = v \cos(\psi + \beta)  \\ 
    \dot{y} =  v \sin(\psi + \beta) \\
    \dot{\psi} = \frac{v}{l_r} \sin{\beta}
\end{cases}
\Rightarrow
\begin{cases} 
    \tau_{t} = [x_t,y_t,\psi_t]^T \\
    a_{t} = [\dot{x}_t,\dot{y}_t,\dot{\psi}_t]^T \\
    u_{t} = [v_t , \beta_t]^T
\end{cases}
\Rightarrow
\begin{cases} 
    \tau_{t+1} = \tau_t + a_t \Delta t \\
    a_{t+1} = u_t + \dot{u} \Delta_t \\
    a_{t} = f(u_t,\dot{u}_t, \tau_t)
\end{cases}
$$

* $x$, $y$ are the coordinates of the center of mass
* $\psi$ is the inertial heading
* $v$ is the speed of the vehicle. 
* $\beta$ is the angle of the current velocity of the center of mass with respect to the longitudinal axis of the car


### 3. Loss Function
* Wasserstein generative learning
* optimization problem:
![-w507](media/16105146218643/16107202643215.jpg)
* Loss function:
![-w464](media/16105146218643/16107202966487.jpg)



## Social NCE: Contrastive Learning of Socially-aware Motion Representations
![-w1124](media/16105146218643/16107026038216.jpg)
This paper proposes a social contrastive learning method to incorporate prior knowledge into motion representation learning. It adapts this learning approach in the multi-agent context and introduce Social-NCE as an auxiliary loss. Social-NCE encourages the extracted motion representation to preserve sufficient information for distinguishing a positive future event from a set of synthetic knowledge-driven negative events.

### 1. Contrastive Representation Learning
**InfoNCE loss:** Maximise the lower bound on the mutual information between the raw input and the latent representation.
$$L_{NCE} = -\log{\frac{\exp(sim(q,k^+)/\tau)}{\sum_{n=0}^n \exp(sim(q,k_n)/\tau)}} \space \textbf{where} \space sim(u,v) = \frac{u^Tv}{||u||\cdot ||v||}$$

* $\tau$: temperature hyperparameter
* $q$: encoded query

### 2. Social NCE

$$L_{\text{Social NCE}} = -\log{\frac{\exp(\psi(h_i) \cdot \phi(s^i_{t+\delta t}, \delta t)/\tau)}{\sum_{n=0}^n \exp(\exp(\psi(h_i) \cdot \phi(s^i_{t+\delta t}, \delta t)/\tau)}} \space $$

* query: $q = \psi(h_i)$
* key: $k = \phi(s^i_{t+\delta t}, \delta t)$ where $s^i_{t+\delta t} = g(h_i)$ for the future path.
* $\psi$,$\phi$ are MLP layers

**Full training objective**:
$$ L(f,g,\psi,\phi) = L_{task}(f,g) + \lambda L_{\text{Social NCE}} $$

* $L_{task}(f,g)$ can be any convention task loss such as $L_{L_2}$ or Negative Log-Likelihood

### 3. Multi-agent Contrastive Sampling
* Draw a set of negative samples from the neighborhood of other agents in the future at time $t + \delta t$:
    $$
    s_{t + \delta t}^{i,n-} = s^j_{t+\delta t} + \Delta s_p + \epsilon
    $$
    * $j\in \{ 1,2,\cdots, M \}/ i$ is the index of other agents
    * $\Delta s_p = (\rho \cos \theta_p, \rho \sin  \theta_p )$



## Human Trajectory Forecasting in Crowds: A Deep Learning Perspective
This paper presents an in-depth analysis of existing deep learning-based methods for modelling social interactions. It proposes two knowledge-based data-driven methods to effectively capture these social interactions.

### Grid Based Interaction Module


### Non-Grid Based Interaction Module


## Recursive Social Behavior Graph for Trajectory Prediction
![-w1027](media/16105146218643/16107262487372.jpg)
This paper presents a novel insight of group-based social interaction model to explore relationships among pedestrians. It recursively extract social representations supervised by group-based annotations and formulate them into a social behaviour graph, called Recursive Social Behavior Graph. Its recursive mechanism explores the representation power largely. Graph Convolutional Neural Network then is used to propagate social interaction information in such a graph.

### 1. Individual Representation
* Historical Trajectory feature
    * Vanilla LSTM $\rightarrow$ BiLSTM

* Human context feature    
    * For each time $t$, a image patch $s_i^t$ centered on $(x_i^t,y_i^t)$ is fed to $CNN$ to $V_i$
    
### 2. Relational Social Representation
* Relational Labeling:
    * using 0/1 to represent whether two pedestrians are in the same group 
    * Experts with sociology background determined
* Feature design
    * Relation map:  $R = softmax(g_s(F)g_o(F)^T) \in R^{N\times N}$ 
    * Feature map $f_i \in F \in R^{N \times L}$
    * $g_s$ and $g_o$ are fully connection network

### 3. Recursive Social Behaviour Graph
$$
    \begin{aligned}
        &R_k = softmax(g_s(F_k)g_o(F_k)^T) \in R^{N\times N}\\
        \text{with} \space &F_{k+1} = fc(F_k + R_kF_k)
    \end{aligned}
$$
* For initialization, features in $F_0$ are historical trajectories in global coordinate.
* $k$ is the depth

$$
    \newenvironment{rcases}
      {\left.\begin{aligned}}
      {\end{aligned}\right\rbrace}
      \begin{aligned}
    \begin{rcases}
    R_a = Avg( \{R_i \rvert i =0\cdots n \}) \\ \\
   \mathcal{V} = \{v_i = t_i \rvert 0\le i \le n\} \\\\
   \mathcal{E} = \{e_{i_1 i_2} = R_a(i_1,i_2) \rvert 0 \le i_1, i_2 < n,  i_1\neq i_2\}\\
    \end{rcases}
    &\Longrightarrow 
     \mathcal{G}_{RSB} = (\mathcal{V},\mathcal{E}) & \\\\     \textbf{where} \space R_a(i_1,i_2) \space \textbf{represents the value in row } &i_1 \textbf{ and column }i_2
    \end{aligned}
 $$
 
### 4. Trajectory Generation
$$
\begin{aligned}
\textbf{step 1:} \space v_i^m &= Relu(fc(GCN(v_j^{m-1},e_{i,j}))) \\
\textbf{step 2:} \space u_i &= v_i^2 \text{ for social representation}\\
\textbf{step 3:} \space \hat{Y}^t_i &= LSTM(h_i^t) \text{ with } \space h_i^0 = [f_i,u_i]
\end{aligned}
$$

### 5. Loss
Exponential $L_2$ loss to consider FDE: $$L_{EL_2} = ||\hat{Y}_i^t - Y_i^t||^2 \times e^\frac{t}{\gamma}$$


## Social and Scene-Aware Trajectory Prediction in Crowded Spaces

![](media/16105146218643/16108217493744.jpg)
This paper constructs an LSTM (long short-term memory)-based model considering three fundamental factors: people interactions, past observations in terms of previously crossed areas and semantics of surrounding space. The model encompasses several pooling mechanisms to join the above elements defining multiple tensors, namely social, navigation and semantic tensors. 

### Navigation Tensor


### Semantic Tensor


### Social Tensor


## SR-LSTM: State Refinement for LSTM towards Pedestrian Trajectory Prediction
![-w674](media/16105146218643/16108880554536.jpg)

> Many methods rely on previous neighboring hidden states but ignore the important current intention of the neighbors. 

This paper proposes a data-driven state refinement module for LSTM network (SR-LSTM), which activates the utilization of the current intention of neighbors, and jointly and iteratively refines the current states of all participants in the crowd through a message passing mechanism. To effectively extract the social effect of neighbors, it further introduces a social-aware information selection mechanism consisting of an element-wise motion gate and a pedestrian-wise attention to select useful message from neighboring pedestrians.


### 1. SR-LSTM Framework

* Vanilla cell state in LSTM 
$$
    c_i^t = g_i^{f,t} \odot c_i^{t-1} + g_i^{u,t} \odot g_i^{c,t}
$$
    * $g$ donate the gate function


* Cell state in SR-LSTM
$$
    \hat{c}_i^{t,l+1} = \sum_{j\in N(i)} M_j (\hat{h}_j^{t,l},\hat{h}_i^{t,l}) + \hat{c}_i^{t,l}
$$
    * $M$ is the message passing function
    * $N(i)$ donates the neighbours of pedestrain $i$
    * $l$ denotes the message passing iteration index.

### 2. Message Passing Function

$$
 M(j) = \frac{W^{mp} \hat{h} _j^{t,l}}{\|N_i\|}
$$

Here
* The $$\|N_i\|$$ donates the number of elements in $N(i)$
* The $W^{mp}$ is a linear transformation using for transmitting the message from neighboring pedestrians to the pedestrian $i$.

### 3. Social-aware information selection

$$
    \begin{aligned}
        \hat{c}_i^{t,l+1} &= \sum_{j\in N(i)} M_j (\hat{h}_j^{t,l},\hat{h}_i^{t,l}) + \hat{c}_i^{t,l} \\
        &= \sum_{j\in N(i)} W^{mp} \alpha_{i,j}^{t,l} \cdot (g_{i,j}^{m,t,l} \odot \hat{h}_j^{t,l})+ \hat{c}_i^{t,l}
    \end{aligned}
$$

* **Pedestrian-wise attention** $ \alpha_{i,j}^{t,l} $ is attention weight vector
    $$
        \alpha_{i,j}^{t,l} = \frac{\exp( u_{i,j}^{t,l})}{\sum_{k} \exp(u_{i,k}^{t,l})}\space\text{where}\space u_{i,j}^{t,l} = w^{aT} [r_{i,j}^{t,k},\hat{h}_{i}^{t,k},h_{j}^{t,k}]
    $$
    * The relative spatial location $r_{i,j}^{t,k} = \phi _r (x_i^t - x_j^t, y_i^t - y_j^t; W^T) $

* **Motion gate**
    $$g_{i,j}^{t,k} = \sigma (W^m [r_{i,j}^{t,k},\hat{h}_{i}^{t,k},h_{j}^{t,k}] + b^m)$$
    
    
## Multi-Agent Tensor Fusion for Contextual Trajectory Prediction
![-w549](media/16105146218643/16108983717809.jpg)
Multi-Agent Tensor Fusion(MATF) encodes multiple agents’ past trajectories and the scene context into a Multi-Agent Tensor, then applies convolutional fusion to capture multi-agent interactions while retaining the spatial structure of agents and the scene context. The model decodes recurrently to multiple agents’ future trajectories, using adversarial loss to learn stochastic predictions. 

### 1.Scene and Social Feature generation
1. The outputs of the LSTM encoders are 1-D agent state vectors: $ \{x_1', x_2', \cdots, x_n' \} = LSTM(\{x_1, x_2, \cdots, x_n \})$ at time $t = t_{final}$.
    
2. The output of the scene context encoder $CNN$ is a scaled feature map $c' = CNN(I)$ retaining the spatial structure of the bird’s-eye view static scene context image.


### 2. Tensor Fusion
1. Agent encodings $\{x_1', x_2', \cdots, x_n' \}$ are placed into one bird’s-eye view spatial tensor, which is initialized to 0 and is of the same shape (width and height) as the encoded scene image $c′$.

2. The agent encodings are placed into the spatial tensor with respect to their positions at the last time step of their past trajectories. 

3. This tensor is then concatenated with the encoded scene image in the channel dimension to get a combined tensor, say Multi-agent Tensor. 

### 3. Interaction Learning 
1. U-Net-like architectures to model interaction at different spatial scales: $C'' = CNN(C')$ with retaining shape.

### 4. Decoding
1. The fused interaction features for each agent $\{ x_1'', x_2'', \cdots, x_n'' \}$ are extracted according to their coordinates on $C''$
 
2. The final agent encoding vectors $\{ x_1' + x_1'', x_2' + x_2'', \cdots, x_n' + x_n'' \}$

3. Finally, the final agent encoding vectors are sent to LSTM to get $\hat{y}_i$.


## Looking to Relations for Future Trajectory Forecast
![-w1230](media/16105146218643/16109025883681.jpg)

The main contributions of this paper are as follows:
1. Encoding of spatio-temporal behavior of agents and their interactions toward environments, corresponding to human-human and human-space interactions.

2. Design of relation gating process conditioned on the past motion of the target to capture more descriptive relations with a high potential to affect its future

3. Prediction of a pixel-level probability map that can be penalized with the guidance of spatial dependencies and extended to learn the uncertainty of the problem.

4. Improvement of model performance by 14−15% over the best state-of-the-art method using the proposed framework with aforementioned contributions.

### 1. Spatio-Temporal Interactions
* Spatial representations: $S = \{s_1,s_2,\cdots,s_n \} = CNN2D(I_t) \in \mathbb{R}^{\tau \times d \times d \times c}$

* Spatio-temporal features: $O = CNN3D(S)$

* the joint use the joint use of 2D conv for spatial  modelling and 3D for temporal model outperforms methods:
    * 3D for all
    * 2D + LSTM

### 2. Relation Gate Module:
![-w648](media/16105146218643/16109042102078.jpg)

*  relational features $F^k \in \mathbb{R}^{1 \times w} $

### 3. Trajectory Prediction Network
* Heatmap $\hat{H} _A^k = a _{\psi}(F^k)$ where $a _{\psi} $ is a set of deconvolutional layers with Relu.

*  Corrected using $L_2$ loss


### 4. Refinement with Spatial Dependencies
* Problem: a lack of spatial dependencies among heatmap predictions

### 5.Uncertainty of Future Prediction
* Embeds the uncertainty of future prediction by adopting Monte Carlo (MC) dropout 