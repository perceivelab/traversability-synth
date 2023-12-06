<div align="center">    
 
# Terrain Traversability Prediction through Self-Supervised Learning and Unsupervised Domain Adaptation on Synthetic Data     
[Giuseppe Vecchio](https://github.com/giuvecchio), [Simone Palazzo](https://github.com/simopal6), Dario C. Guastella, Daniela Giordano, Giovanni Muscato and Concetto Spampinato

<!--
[![Paper](http://img.shields.io/badge/paper-arxiv.2107.11298-B31B1B.svg)](https://arxiv.org/abs/2107.11298)
[![Conference](http://img.shields.io/badge/ICCV-2021-4b44ce.svg)](https://openaccess.thecvf.com/content/ICCV2021/html/Vecchio_SurfaceNet_Adversarial_SVBRDF_Estimation_From_a_Single_Image_ICCV_2021_paper.html)
--> 

<!--  
Conference   
-->   
</div>
 
## Overview   
This is the official repo for paper __"Terrain Traversability Prediction through Self-Supervised Learning and Unsupervised Domain Adaptation on Synthetic Data"__.

Dataset, code, and additional resources will be made available here.

<br/>

<!--![alt text](https://github.com/perceivelab/surfacenet/blob/main/imgs/hd_sample.jpg?raw=true)-->

<!--![alt text](https://github.com/perceivelab/surfacenet/blob/main/imgs/figures/framework.png?raw=true)-->

## Abstract

Terrain traversability estimation is a fundamental task for supporting robot navigation on uneven surfaces. Recent approaches based on deep models for predicting traversability from RGB images have shown promising results; however, supervised training of such models requires manual annotation of a large number of images. In this paper, we present a learning approach for traversability estimation on unlabeled videos by combining dataset synthesis (with computer-generated annotations), self-supervision and unsupervised domain adaptation.
Our method poses traversability estimation as a vector regression task over vertical portions of the observed scene. The regression model is first pre-trained through self-supervision to reduce the distribution shift between synthetic and real data and encourage shared feature learning. Then, the model is trained in a supervised way on synthetic videos, while employing an unsupervised domain adaptation loss, by means of gradient reversal, to improve its generalization capabilities on real scenes. 
Experimental on-field results show that our approach is able to achieve an estimation accuracy on par with standard supervised training, without the need to carry out manual annotation.

## Method
![alt text](https://github.com/perceivelab/traversability-synth/blob/78aee5dd0e477ca290456b536f839e62713ab771/img/TravFramework.png?raw=true)
<!--
## Instructions   
First, install dependencies   
```bash
# clone project   
git clone https://github.com/perceivelab/surfacenet

# install requirements 
cd surfacenet
pip install -r requirements.txt
 ```   
 Next, navigate to the main and run it to strat the training.   
 ```bash
# module folder
cd surfacenet

# run training   
python main.py    
```
-->

## Dataset

The dataset employed in the experiments reported in the paper is available [at this link](https://studentiunict-my.sharepoint.com/:u:/g/personal/simone_palazzo_unict_it/EbylSagC91ZAnIHNYuTVYFcB9X1qLQ8P62fAS20Ws83jdA?e=W5m9vS) (1.42 GB zip file).

<!--
### Citation   
```
@inproceedings{vecchio2021surfacenet,
  title={SurfaceNet: Adversarial SVBRDF Estimation from a Single Image},
  author={Vecchio, Giuseppe and Palazzo, Simone and Spampinato, Concetto},
  booktitle={Proceedings of the IEEE/CVF International Conference on Computer Vision},
  pages={12840--12848},
  year={2021}
}
```   
-->
