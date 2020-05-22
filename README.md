# Easy Regions First: Self-paced Learning for Integrate Salient Object Detection

## abstract

Accurately segment the integral salient object is very challenging due to the heterogeneous of salient regions in terms of their illumination, texture, and contrast. In this paper,  we propose a simple yet effective framework to address this problem. On the one hand, we propose a novel two-stream structure to discover the complementary object regions by using two independent  supervisor and obtain relatively complete salient regions. On the other hand, instead of segmenting entire salient regions at one time, we introduce self-paced adversarial learning algorithm for localizing and mining salient regions progressively. By adapting the weight of the salient regions, our self-paced adversarial learning  algorithm can train multiple complementary saliency networks sequentially, where each of them focuses on mining new salient regions ignored by previous stage in an easy-to-hard way. With such a self-paced learning, we can finally produce integral salient regions. Extensive experiments on five datasets show that the proposed model outperforms 14 state-of-the-art methods. In addition, the attribute-based performance on the SOC dataset also demonstrate the superiority of our approach.


## Network architecture

![fig1](./img/pipeline.png)


##Requirements
- Python 3.5
-  OpenCV
- PyTorch 0.4

### Visual comparison with previous start-of-the-arts

![fig1](./img/sal_maps.png)

### PR and F-measure curves
![fig2](./img/pr.png)

###  Comparison of quantitative results including the F-measure and MAE
![fig3](./img/tab.png)
