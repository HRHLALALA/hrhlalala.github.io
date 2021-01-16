---
title: Trajectory Prediction Paper Literature Review
date: '2021-01-14'
layout: post
thumb_image: images/SE-GAN.png
toc: true
---
| Paper                                                                                                      | Year | Conference | Keywords                                                                                                           | link                                                                                                                                                                                         | Code                                                        |
| ---------------------------------------------------------------------------------------------------------- | ---- | ---------- | ------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------- |
| CoL-GAN: Plausible and Collision-Less Trajectory Prediction by Attention-Based GAN                         | 2020 | IEEE       | CNN-Based Discriminator; Attention Module in Decoder; Relative position and speed as Attention Input               | [link](https://ieeexplore.ieee.org/ielx7/6287639/8948470/09063432.pdf)                                                                                                                       |                                                             |
| DAG-Net: Double Attentive Graph Neural Network for Trajectory Forecasting                                  | 2020 | ICPR       | Recurrent VAE;                                                                                                     | [link](https://arxiv.org/pdf/2005.12661.pdf)                                                                                                                                                 | [link](https://github.com/alexmonti19/dagnet)               |
| Dynamic and Static Context-aware LSTM for Multi-agent Motion Prediction                                    | 2020 | ECCV       | Individual Context Module; Social Aware Context Module; Sematntic Guidence; Temporal Correlation Coefficient       | [link](https://arxiv.org/pdf/2008.00777.pdf)                                                                                                                                                 |                                                             |
| EvolveGraph: Multi-Agent Trajectory Prediction with Dynamic Relational Reasoning,                          | 2020 | NeurIPS    |                                                                                                                    | [link](https://arxiv.org/pdf/2003.13924.pdf)                                                                                                                                                 |                                                             |
| Goal-driven Long-Term Trajectory Prediction                                                                | 2021 | WACV       | Goal Channel; Controller sub-network                                                                               | [link](https://openaccess.thecvf.com/content/WACV2021/papers/Tran_Goal-Driven_Long-Term_Trajectory_Prediction_WACV_2021_paper.pdf)                                                           |                                                             |
| Goal-GAN:Multimodal Trajectory Prediction Based on Goal Position Estimation                                | 2020 | ACCV       | Goal Estimation; Routing Module; Gumbel Sampling; Attn Decoder; GAN;                                               | [link](https://arxiv.org/pdf/2010.01114.pdf)                                                                                                                                                 | [link](https://github.com/dendorferpatrick/GoalGAN)         |
| GraphTCN: Spatio-Temporal Interaction Modeling for Human Trajectory Prediction                             | 2021 | WACV       | Edge feature based graph attention network(EFGAT); Temporal convolutional network(TCN);                            | [link](https://openaccess.thecvf.com/content/WACV2021/papers/Wang_GraphTCN_Spatio-Temporal_Interaction_Modeling_for_Human_Trajectory_Prediction_WACV_2021_paper.pdf)                         |                                                             |
| How Can I See My Future? FvTraj: Using First-person View for Pedestrian Trajectory Prediction              | 2020 | ECCV       |                                                                                                                    | [link](http://graphics.cs.uh.edu/wp-content/papers/2020/2020-ECCV-PedestrianTrajPrediction.pdf)                                                                                              |                                                             |
| Human Trajectory Forecasting in Crowds: A Deep Learning Perspective                                        | 2020 | ArXiv      |                                                                                                                    | [link](https://arxiv.org/pdf/2007.03639.pdf)                                                                                                                                                 |                                                             |
| It is not the Journey but the Destination- Endpoint Conditioned Trajectory Prediction;Truncation Trick     | 2020 | ECCV       | Goal-based method; VAE; KL Divergence Loss; Average Endpoint Los, Average Trajctory Loss; Non-Local Social Pooling | [link](https://arxiv.org/pdf/2004.02025.pdf)                                                                                                                                                 |                                                             |
| Recursive Social Behavior Graph for Trajectory Prediction                                                  | 2020 | CVPR       | CNN for Patch Image Input; BiLSTM; GCN; Handcraft Group Annotation; Exponential Loss                               | [link](https://openaccess.thecvf.com/content_CVPR_2020/papers/Sun_Recursive_Social_Behavior_Graph_for_Trajectory_Prediction_CVPR_2020_paper.pdf)                                             |                                                             |
| Self-Growing Spatial Graph Networks for Pedestrian Trajectory Prediction                                   | 2020 | WACV       | Spatial Graphic Network; Multiple Stacked GRU; motion features;                                                    | [link](https://openaccess.thecvf.com/content_WACV_2020/papers/Haddad_Self-Growing_Spatial_Graph_Networks_for_Pedestrian_Trajectory_Prediction_WACV_2020_paper.pdf)                           |                                                             |
| SILA: An Incremental Learning Approach for Pedestrian TrajectoryPrediction.                                | 2020 | CVPR       | Similarty -based Icremental Learning Algorithm; Speed Improve;                                                     | [link](https://openaccess.thecvf.com/content_CVPRW_2020/papers/w66/Habibi_SILA_An_Incremental_Learning_Approach_for_Pedestrian_Trajectory_Prediction_CVPRW_2020_paper.pdf)                   |                                                             |
| SMART: Simultaneous Multi-Agent Recurrent Trajectory Prediction                                            | 2020 | ECCV       |                                                                                                                    | [link](https://arxiv.org/pdf/2007.13078.pdf)                                                                                                                                                 |                                                             |
| Social NCE: Contrastive Learning of Socially-aware Motion Representations.                                 | 2020 | NeurIPS    |  Contrastive Represent Learning; InfoNCE Loss; Contrastive Sampling                                                | [link](https://arxiv.org/pdf/2012.11717.pdf)                                                                                                                                                 | [link](https://github.com/vita-epfl/social-nce)             |
| Social-STGCNN: A Social Spatio-Temporal Graph Convolutional Neural Network for Human Trajectory Prediction | 2020 | CVPR       | GCNN;                                                                                                              | [link](https://openaccess.thecvf.com/content_CVPR_2020/papers/Mohamed_Social-STGCNN_A_Social_Spatio-Temporal_Graph_Convolutional_Neural_Network_for_Human_CVPR_2020_paper.pdf)               | [link](https://github.com/abduallahmohamed/Social-STGCNN)   |
| Social-WaGDAT: Interaction-aware Trajectory Prediction via Wasserstein Graph Double-Attention Network      | 2020 | ArXiv      | Two GAT system; Kinematic Constraint;Wasserstein generative learning                                               | [link](https://arxiv.org/pdf/2002.06241.pdf)                                                                                                                                                 |                                                             |
| Spatio-Temporal Graph Transformer Networks for Pedestrian Trajectory Prediction                            | 2020 | ECCV       | Transformer Network; TGConv; 2-encoder structure; Graph Memory                                                     | [link](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123570494.pdf)                                                                                                               | [link](https://github.com/Majiker/STAR)                     |
| The Garden of Forking Paths: Towards Multi-Future Trajectory Prediction                                    | 2020 | CVPR       | multi-scale location encodings; convolutional RNNs over graphs                                                     | [link](https://openaccess.thecvf.com/content_CVPR_2020/papers/Liang_The_Garden_of_Forking_Paths_Towards_Multi-Future_Trajectory_Prediction_CVPR_2020_paper.pdf)                              |                                                             |
| Trajectron++: Dynamically-Feasible Trajectory Forecasting With Heterogeneous Data                          | 2020 | ECCV       |                                                                                                                    | [link](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123630664.pdf)                                                                                                               | [link](https://github.com/StanfordASL/Trajectron-plus-plus) |
| Multiple Futures Prediction                                                                                | 2019 | NeurIPS    |                                                                                                                    | [link](http://papers.nips.cc/paper/9676-multiple-futures-prediction.pdf)                                                                                                                     |                                                             |
| STGAT: Modeling Spatial-Temporal Interactions for Human Trajectory Prediction                              | 2019 | ICCV       | GAT; Spatio-temporal                                                                                               | [link](http://openaccess.thecvf.com/content_ICCV_2019/papers/Huang_STGAT_Modeling_Spatial-Temporal_Interactions_for_Human_Trajectory_Prediction_ICCV_2019_paper.pdf)                         |                                                             |
| Social and Scene-Aware Trajectory Prediction in Crowded Spaces                                             | 2019 | ICCV       |                                                                                                                    | [link](https://arxiv.org/pdf/1909.08840.pdf)                                                                                                                                                 | [link](https://github.com/Oghma/sns-lstm/)                  |
| PIE: A Large-Scale Dataset and Models for Pedestrian Intention Estimation and Trajectory Prediction        | 2019 | ICCV       |                                                                                                                    | [link](https://openaccess.thecvf.com/content_ICCV_2019/papers/Rasouli_PIE_A_Large-Scale_Dataset_and_Models_for_Pedestrian_Intention_Estimation_ICCV_2019_paper.pdf)                          | [link](https://github.com/huang-xx/STGAT)                   |
| Trajectory Prediction by Coupling Scene-LSTM with Human Movement LSTM                                      | 2019 | ISVC       |                                                                                                                    | [link](https://arxiv.org/pdf/1908.08908.pdf)                                                                                                                                                 |                                                             |
| Scene Compliant Trajectory Forecast with Agent-Centric Spatio-Temporal Grids                               | 2019 | ArXiv      |                                                                                                                    | [link](https://arxiv.org/pdf/1909.07507.pdf)                                                                                                                                                 |                                                             |
| trajectory Prediction of Mobile Construction Resources Toward Pro-active Struck-by Hazard Detection        | 2019 | ISARC      |                                                                                                                    | [link](https://www.iaarc.org/publications/fulltext/ISARC_2019_Paper_201.pdf)                                                                                                                 |                                                             |
| Learning to Infer Relations for Future Trajectory Forecast                                                 | 2019 | CVPR       |                                                                                                                    | [link](https://openaccess.thecvf.com/content_CVPRW_2019/papers/Precognition/Choi_Learning_to_Infer_Relations_for_Future_Trajectory_Forecast_CVPRW_2019_paper.pdf)                            |                                                             |
| Looking to Relations for Future Trajectory Forecast                                                        | 2019 | ICCV       |                                                                                                                    | [link](https://openaccess.thecvf.com/content_ICCV_2019/papers/Choi_Looking_to_Relations_for_Future_Trajectory_Forecast_ICCV_2019_paper.pdf)                                                  |                                                             |
| Multi-Agent Tensor Fusion for Contextual Trajectory Prediction                                             | 2019 | CVPR       |                                                                                                                    | [link](https://openaccess.thecvf.com/content_CVPR_2019/papers/Zhao_Multi-Agent_Tensor_Fusion_for_Contextual_Trajectory_Prediction_CVPR_2019_paper.pdf)                                       |                                                             |
| SR-LSTM: State Refinement for LSTM towards Pedestrian Trajectory Prediction                                | 2019 | CVPR       |                                                                                                                    | [link](https://openaccess.thecvf.com/content_CVPR_2019/papers/Zhang_SR-LSTM_State_Refinement_for_LSTM_Towards_Pedestrian_Trajectory_Prediction_CVPR_2019_paper.pdf)                          | [link](https://github.com/zhangpur/SR-LSTM)                 |
| Social Ways: Learning Multi-Modal Distributions of Pedestrian Trajectories With GANs                       | 2019 | CVPR       | Info GAN                                                                                                           | [link](http://openaccess.thecvf.com/content_CVPRW_2019/papers/Precognition/Amirian_Social_Ways_Learning_Multi-Modal_Distributions_of_Pedestrian_Trajectories_With_GANs_CVPRW_2019_paper.pdf) | [link](https://github.com/amiryanj/socialways)              |

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
![-w758](media/16105146218643/16105207586767.jpg)
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
* **TGConv**
    * A transformer version of GAT 
$$
Attn(Q,K,V) = \frac{Softmax([m^{j\rightarrow i}]_{i,j = 1:n})}{\sqrt{dk}}[v_i]_{i=1}^{n}\\
\textbf{where the message from node j to i in the fully connected graph}\\ \space m^{j\rightarrow i} = q_i^Tk_j
$$



### 3. Spatio-Temporal Graph Transformer
* Encoder 1:
    * To extract independent spatial and temporal information from the pedestrian history.

* Encoder 2:
    * spatial Transformer models spatial interaction with temporal information; 
    * the temporal Transformer enhances the output spatial embeddings with temporal attentions. 

    
### 4. External Graph Memory
* In encoder 1, the temporal Transformer ﬁrst reads from memory $M$ the past graph embeddings $ \{\tilde{h} _1, \tilde{h} _2,\cdots, \tilde{h} _{t-1}\} $ and concatenate it with the current graph embedding $h_t$.

  $$
    \{\tilde{h}_1,\tilde{h}_2,\cdots,\tilde{h}_{t-1}\} = f_{read}(M) = \{M_1,M_2,M_3,\cdots,M_{t-1}\}
  $$
  
* In encoder 2,  the output of Temporal Transformer is written to the graph memory which performs a smoothing over the time series data.   
$$ 
  M' = f_{write}(\{h'_1,h'_2,\cdots,h'_i\},M) =\{h'_1,h'_2,\cdots,h'_i\}
$$

## It is not the Journey but the Destination: Endpoint Conditioned Trajectory Prediction
![-w1167](media/16105146218643/16107203965010.jpg)

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


## Social-WaGDAT: Interaction-aware Trajectory Prediction via Wasserstein Graph Double-Attention Network
![-w840](media/16105146218643/16107019503809.jpg)
### 1.  Feature Extraction
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


## Recursive Social Behavior Graph for Trajectory Prediction
![-w1027](media/16105146218643/16107262487372.jpg)
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
 