# Crafting Object Detection in Very Low Light

This is Low-light Object Detection (LOD) dataset and reference code of Crafting Object Detection in Very Low Light in BMVC(British Machine Vision Conference) 2021, by Yang Hong, Kaixuan Wei, Linwei Chen, and Ying Fu (Continuously updating).

------

**Paper**

------



## Representitive Example Scenes of LOD

![](https://cdn.jsdelivr.net/gh/MUYIio/CDN@2.0/Images/Paper/1.png)



## Environment Preparing

The code is tested on Python 3.7, PyTorch 1.7.0, TorchVision 0.8.1, but lower versions are also likely to work.



## Realistic Low-light Synthetic Pipeline

**Description**

You can use our pipline from **here** transform annotated images from existing object detection datasets(e.g., Pascal VOC, COCO) into their low-light counterparts. Feel free to replace our unprocessing or noise injection model for all of your data synthesis needs.

**Overal pipline**

![](https://cdn.jsdelivr.net/gh/MUYIio/CDN@2.0/Images/Paper/2.png)



## Low-light Object Detection (LOD) Dataset

1. RGB-normal(long-exposure normal-light images in sRGB format) images with annotations: 

**[BaiduYun_RGB-normal]**

2. RGB-dark(short-exposure low-light images in sRGB format) images with annotations: 

**[BaiduYun_RGB-dark]**

3. RAW-normal(long-exposure normal-light images in RAW format) images with annotations: 

**[BaiduYun_RAW-normal]**

4. RAW-dark(short-exposure low-light images in RAW format) images with annotations: 

**[BaiduYun_RAW-dark]**

 

### Tips:

1. Note that each short-exposure image correspond to one long-exposure image as Ground Truth.

2. We provide the camera output raw data of Canon EOS 5D Mark IV camera so that you can process the data in a different way, but the original raw data is much larger. 

3. We name all images with a purely numeric number, paired long/short-exposure images file names of the same format are corresponding(short-exposure image file name= long -exposure image file name+1). For example, for “1.JPG”, the file name of the corresponding short exposure image is “2. JPG”; for “11.JPG”, the file name of the corresponding long exposure image is “12.CR2”.



## Citation

If you use our dataset or code for research, please ensure that you cite our paper:

Yang Hong, Kaixuan Wei, Linwei Chen, and Ying Fu, "Crafting Object Detection in Very Low Light", in BMVC, 2021.

```
@inproceedings{Hong2021Crafting,
	title={ Crafting    Object Detection in Very Low Light },     
	author={ Yang    Hong, Kaixuan Wei, Linwei Chen, Ying Fu },     
	booktitle={British Machine Vision    Conference},     
	year={2021},     
	organization={British Machine Vision    Association} 
}   
```



## Questions

If you have any questions about our dataset and code, please email to hongyang@bit.edu.cn