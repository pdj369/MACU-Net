# MACU-Net: Semantic Segmentation from High-Resolution Remote Sensing Images 

In this repository, we incorporate multi-scale features generated by different layers of U-Net and design a multi-scale skip connected and asymmetric-convolution-based U-Net (MACU-Net), for segmentation using fine-resolution remotely sensed images. 

The detailed results can be seen in the [MACU-Net Semantic Segmentation from High-Resolution Remote Sensing Images](https://arxiv.org/ftp/arxiv/papers/2007/2007.13083.pdf).

Feel free to contact me if you need any further information: lironui@163.com

If our code is helpful to you, please cite:

`Li, Rui, Chenxi Duan, and Shunyi Zheng. "MACU-Net Semantic Segmentation from High-Resolution Remote Sensing Images." arXiv preprint arXiv:2007.13083 (2020).`

`Li, Rui, et al. "Multistage Attention ResU-Net for Semantic Segmentation of Fine-Resolution Remote Sensing Images." arXiv preprint arXiv:2011.14302 (2020).`

Requirements：
------- 
```
numpy >= 1.16.5
PyTorch >= 1.3.1
sklearn >= 0.20.4
tqdm >= 4.46.1
glob >= 
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

You can download the hyperspectral datasets in mat format at: http://www.ehu.eus/ccwintco/index.php/Hyperspectral_Remote_Sensing_Scenes, and move the files to `./datasets` folder.
