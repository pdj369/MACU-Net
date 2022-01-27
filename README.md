# MACU-Net for Semantic Segmentation of Fine-Resolution Remotely Sensed Images 

⭐ [Welcome to my HomePage](https://lironui.github.io/) ⭐ 

In this repository, we incorporate multi-scale features generated by different layers of U-Net and design a multi-scale skip connected and asymmetric-convolution-based U-Net (MACU-Net), for segmentation using fine-resolution remotely sensed images. 

The detailed results can be seen in the [MACU-Net for Semantic Segmentation of Fine-Resolution Remotely Sensed Images](https://ieeexplore.ieee.org/document/9343296).

If our code is helpful to you, please cite:

`R. Li, C. Duan, S. Zheng, C. Zhang and P. M. Atkinson, "MACU-Net for Semantic Segmentation of Fine-Resolution Remotely Sensed Images," in IEEE Geoscience and Remote Sensing Letters, doi: 10.1109/LGRS.2021.3052886.`

`R. Li, S. Zheng, C. Duan, J. Su and C. Zhang. "Multistage Attention ResU-Net for Semantic Segmentation of Fine-Resolution Remote Sensing Images." in IEEE Geoscience and Remote Sensing Letters, doi: 10.1109/LGRS.2021.3063381.`

Requirements：
------- 
```
numpy >= 1.16.5
PyTorch >= 1.3.1
sklearn >= 0.20.4
tqdm >= 4.46.1
imageio >= 2.8.0
```

Datasets:
------- 
* [GID](https://x-ytong.github.io/project/GID.html)
* [WHDLD](https://sites.google.com/view/zhouwx/dataset#h.p_hQS2jYeaFpV0)

Note: We select 15 images contained in GID, which cover the whole six categories:
```
GF2_PMS1__L1A0000647767-MSS1
GF2_PMS1__L1A0001064454-MSS1
GF2_PMS1__L1A0001348919-MSS1
GF2_PMS1__L1A0001680851-MSS1
GF2_PMS1__L1A0001680853-MSS1
GF2_PMS1__L1A0001680857-MSS1
GF2_PMS1__L1A0001757429-MSS1
GF2_PMS2__L1A0000607681-MSS2
GF2_PMS2__L1A0000635115-MSS2
GF2_PMS2__L1A0000658637-MSS2
GF2_PMS2__L1A0001206072-MSS2
GF2_PMS2__L1A0001471436-MSS2
GF2_PMS2__L1A0001642620-MSS2
GF2_PMS2__L1A0001787089-MSS2
GF2_PMS2__L1A0001838560-MSS2
```

You can download datasets and prepare the files to `./datasets` folder.
Note: 
```
Transfer the lable images form RGB Format to Grey-scale Map.
Augment the training set by the technology mentioned in our paper.
```

Network:
------- 
![network](https://github.com/lironui/MACU-Net/blob/master/figures/Fig.%201.png)  
Fig. 1.  Comparison of (a) U-Net, (b) U-Net++， and proposed (c) MACU-Net 3+. The depth of each node is presented below the circle. 

Results:
------- 
![Result](https://github.com/lironui/MACU-Net/blob/master/figures/Fig.%204.png)  
Fig. 2. Visualization of results on the WHDLD dataset (the left) and the GID dataset (the right).
