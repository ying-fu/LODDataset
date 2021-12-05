# Crafting Object Detection in Very Low Light

​	This is Low-light Object Detection (LOD) dataset and reference code of Crafting Object Detection in Very Low Light in BMVC(British Machine Vision Conference) 2021, by Yang Hong, Kaixuan Wei, Linwei Chen, and Ying Fu.

------

**Paper**

------



## Representitive Example Scenes of LOD

![](https://cdn.jsdelivr.net/gh/MUYIio/CDN@1.9/Images/Paper/1.png)



## Environment Preparing

The code is tested on Python 3.7, PyTorch 1.7.0, TorchVision 0.8.1, but lower versions are also likely to work.



## Realistic Low-light Synthetic Pipeline

**Description**

You can use our pipline from **here** transform annotated images from existing object detection datasets(e.g., Pascal VOC, COCO) into their low-light counterparts. Feel free to replace our unprocessing or noise injection model for all of your data synthesis needs.

**Overal pipline**

![](https://cdn.jsdelivr.net/gh/MUYIio/CDN@1.9/Images/Paper/2.png)



## Low-light Object Detection (LOD) Dataset

**Images for LOD**

1. RGB-normal(long-exposure normal-light images in sRGB format) images: 

**[RGB-normal-images]** (Extraction Code: 2021)

https://pan.baidu.com/s/1CEFDrd0SeVmsZG_MekzpPQ

2. RGB-dark(short-exposure low-light images in sRGB format) images: 

**[RGB-dark-images]** (Extraction Code: 2021)

https://pan.baidu.com/s/1yilj1ei6nIYsCMkNxLqOFg

3. RAW-normal(long-exposure normal-light images in RAW format) images:

**[RAW-normal-images]** (Extraction Code: 2021)

https://pan.baidu.com/s/1gmkIbr86dKMSs2xBKy6_-A

4. RAW-dark(short-exposure low-light images in RAW format) images:

**[RAW-dark-images]** (Extraction Code: 2021)

https://pan.baidu.com/s/1cWu7Y6GtiRV9itZEbop4VQ

------

## Annotations for LOD

We provide the per-image '.xml' files here: **RGB-normal-Annotations**, **RGB-dark-Annotations**, **RAW-normal-Annotations**, **RAW-dark-Annotations**. (Extraction Code: 2021)

RGB-normal-Annotations: https://pan.baidu.com/s/1mk-qOeofXR5gBT9i1Az04A

RGB-dark-Annotations: https://pan.baidu.com/s/1jJ7jRAD1mrXcjHnvxHTPXA

RAW-normal-Annotations: https://pan.baidu.com/s/14W1U77dslKoQyXme6YsEmw

RAW-dark-Annotations: https://pan.baidu.com/s/1pFAwtaX4ufuZaMy31Sv0AA

 

**Original sensor raw data**

The original raw data is much larger. If you need to process the data in a different way, you can download the camera output raw data here: **all_raw**. (Extraction Code: 2021)

https://pan.baidu.com/s/1phBWWedKwcCJONNhny5_8g

And you can download the camera output original sRGB data here: **all_rgb**.(Extraction Code: 2021)

https://pan.baidu.com/s/1p1lO9KDoNcLih0eIM_kUQQ

### Tips:

1.  \1. We provide all files in **Baidu Drive**, and the extraction code of all files is “2021”.
2. Note that each short-exposure image correspond to one long-exposure image as Ground Truth.
3. We provide the camera output raw data of Canon EOS 5D Mark IV camera so that you can process the data in a different way, but the original raw data is much larger. 
4.  We name all images with a purely numeric number, paired long/short-exposure images file names of the same format are corresponding(short-exposure image file name= long -exposure image file name+1). For example, for “1.JPG”, the file name of the corresponding short exposure image is “2. JPG”; for “11.JPG”, the file name of the corresponding long exposure image is “12.CR2”.
5. Each pair of raw data and rgb data with the same name are capture in the same scene with the same illumination.



## Citation

If you use our dataset or code for research, please ensure that you cite our paper:

Yang Hong, Kaixuan Wei, Linwei Chen, and Ying Fu, "Crafting Object Detection in Very Low Light", in BMVC, 2021.

> @inproceedings{Hong2021Crafting,
>
>  title={Crafting Object Detection in Very Low Light },
>
>  author={Yang Hong, Kaixuan Wei, Linwei Chen, Ying Fu},
>
>  booktitle={BMVC},
>
>  year={2021},

​          



## Questions

If you have any questions about our dataset and code, please email to hongyang@bit.edu.cn