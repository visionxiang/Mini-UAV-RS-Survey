# Mini-Unmanned Aerial Vehicle-Based Remote Sensing: Techniques, Applications, and Prospects (GRSM2019)

<p align="left">
<a href="https://arxiv.org/abs/1812.07770"><img src="https://img.shields.io/badge/Paper-arXiv-green"></a>
<a href="/papers/Mini-UAV-based_RS_MGRS.2019.2918840.pdf"><img src="https://img.shields.io/badge/Paper-PDF-blue"></a>
</p>

This repository contains a collection of research papers and resources for Mini-Unmanned Aerial Vehicle-Based Remote Sensing.  The repository gives a survey of related mini-UAV-based remote sensing, aiming to boost the development of this field.


## Table of Contents
- [Background](#Background)
- [Survey](#Survey)
     - [1. Related Surveys](#1-Related-Surveys)
     - [2. Camera Calibration](#2-Camera-Calibration)
     - [3. Combined Field of View](#3-Combined-Field-of-View)
     - [4. UAV Image Matching](#4-Low-altitude-UAV-image-matching)
     - [5. Low-altitude AAT](#5-Low-altitude-automatic-aerial-triangulation)
     - [6. Dense Reconstruction](#6-Dense-reconstruction)
     - [7. Image Stitching](#7-Image-stitching)
     - [8. Multi-sensor Data Registration](#8-Multi-sensor-data-registration)
     - [9. High-performance Data Processing](#9-High-performance-data-processing)
- [Dataset and Tools](#Dataset-and-Tools) 
- [Citation](#Citation)



## Background

The past few decades have witnessed great progress of unmanned aircraft vehicles (UAVs) in civilian fields, especially in photogrammetry and remote sensing. In contrast with the platforms of manned aircraft and satellites, the UAV platform holds many promising characteristics: flexibility, efficiency, high-spatial/temporal resolution, low cost, easy operation, etc., which make it an effective complement to other remote sensing platforms and a cost-effective means for remote sensing. In light of the popularity and expansion of UAV-based remote sensing in recent years, this paper provides a systematic survey on the recent advances and future prospects of UAVs in the remote-sensing community. 

<div align=center><img src="/figures/intro.png" width="90%"></div>

Specifically, this paper is devoted to present:
- The main challenges and key technologies of remote-sensing data processing based on UAVs are discussed and summarized. 
- A systematic survey of data processing technologies, categorized into eight different themes. In each section, we provide a critical overview of the state-of-the-art, illustrations, current challenges, and possible future works;
- A detailed overview of recent potential applications of UAVs in remote sensing;
- A discussion of the future directions and challenges of UAV-RS from the point of view of platform and technology.

We hope this work will provide remote-sensing researchers an overall picture of recent UAV-based remote sensing developments and help guide further research on this topic.



## Survey

### 1. Related Surveys

| **Year** | **Pub.** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| 2021 | AIR | Applications, databases and open computer vision research from drone videos and images: a survey  <br> <sup><sub>*Younes Akbari, Noor Almaadeed, Somaya Al-maadeed & Omar Elharrouss*</sub></sup>  | [Paper](https://link.springer.com/article/10.1007/s10462-020-09943-1)
| 2019 | GRSM | **Mini-Unmanned Aerial Vehicle-Based Remote Sensing: Techniques, Applications, and Prospects** <br> <sup><sub>*Tian-Zhu Xiang, Gui-Song Xia, Liangpei Zhang*</sub></sup>  | [Paper](https://arxiv.org/abs/1812.07770)
| 2017  | RS | Hyperspectral Imaging: A Review on UAV-Based Sensors, Data Processing, and Applications for Agriculture and Forestry <br> <sup><sub>*Adão, Telmo, Jonáš Hruška, Luís Pádua, José Bessa, Emanuel Peres, Raul Morais, and Joaquim João Sousa*</sub></sup>  | [Paper](https://www.mdpi.com/2072-4292/9/11/1110)
| 2017 | IJRS | UAS, Sensors, and Data Processing in Agroforestry: A Review Towards Practical Applications <br> <sup><sub>*Luís Pádua, Jakub Vanko, Jonáš Hruška, Telmo Adão, Joaquim J. Sousa ORCID Icon, Emanuel Peres & Raul Morais*</sub></sup>  | [Paper](https://www.tandfonline.com/doi/abs/10.1080/01431161.2017.1297548)
| 2017 | IJRS | Forestry Applications of UAVs in Europe: A Review  <br> <sup><sub>*Chiara Torresan, Andrea Berton, Federico Carotenuto, Salvatore Filippo Di Gennaro, Beniamino Gioli, Alessandro Matese, Franco Miglietta, Carolina Vagnoli, Alessandro Zaldei & Luke Wallace*</sub></sup>  | [Paper](https://www.tandfonline.com/doi/abs/10.1080/01431161.2016.1252477)
| 2017 | GRSM | Unmanned Aerial Vehicles and Spatial Thinking: Boarding Education With Geotechnology and Drones <br> <sup><sub>*Arnau Fombuena*</sub></sup>  | [Paper](https://ieeexplore.ieee.org/document/8038992)
| 2017 | RS | Review of the Current State of UAV Regulations  <br> <sup><sub>*Stöcker, Claudia, Rohan Bennett, Francesco Nex, Markus Gerke, and Jaap Zevenbergen*</sub></sup>  | [Paper](https://www.mdpi.com/2072-4292/9/5/459)
| 2017 | IJRS | UAVs: Regulations and Law Enforcement  <br> <sup><sub>*Arthur P. Cracknell*</sub></sup>  | [Paper](https://www.tandfonline.com/doi/abs/10.1080/01431161.2017.1302115)
| 2016 |  RSE | UAVs as Remote Sensing Platform in Glaciology: Present Applications and Future Prospects  <br> <sup><sub>*Anshuman Bhardwaj, Lydia Sam, Akanksha, F. Javier Martín-Torres, Rajesh Kumar*</sub></sup>  | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0034425715302509)
| 2015  | PERS | Overview and Current Status of Remote Sensing Applications Based on Unmanned Aerial Vehicles (UAVs)  <br> <sup><sub>*Gonzalo Pajares*</sub></sup>  | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0099111215300793)
| 2014  | <sup><sub>ISPRS JPRS</sub></sup> | Unmanned Aerial Systems for Photogrammetry and Remote Sensing: A Review  <br> <sup><sub>*I. Colomina, P. Molina*</sub></sup>  | [Paper](https://www.sciencedirect.com/science/article/pii/S0924271614000501)
| 2014 | GISRS | Recent Applications of Unmanned Aerial Imagery in Natural Resource Management  <br> <sup><sub>*Mozhdeh Shahbazi, Jérôme Théau & Patrick Ménard*</sub></sup>  | [Paper](https://www.tandfonline.com/doi/full/10.1080/15481603.2014.926650)
| 2012 | RS | Unmanned Aircraft Systems in Remote Sensing and Scientific Research: Classification and Considerations of Use  <br> <sup><sub>*Watts, Adam C., Vincent G. Ambrosia, and Everett A. Hinkley*</sub></sup>  | [Paper](https://www.mdpi.com/2072-4292/4/6/1671)
| 2011 | GISRS | Small-Scale Unmanned Aerial Vehicles in Environmental Remote Sensing: Challenges and Opportunities  <br> <sup><sub>*Perry J. Hardin, Ryan R. Jensen*</sub></sup>  | [Paper](https://www.tandfonline.com/doi/abs/10.2747/1548-1603.48.1.99)
| :triangular_flag_on_post: | `Geometry` |  | 
| 2022 | GRSM | Unmanned Aerial Vehicle-Based Photogrammetric 3D Mapping: A survey of techniques, applications, and challenges  <br> <sup><sub>*San Jiang; Wanshou Jiang; Lizhe Wang*</sub></sup> | [Paper](https://ieeexplore.ieee.org/abstract/document/9627932)
| 2016 | <sup><sub>ISPRS JPRS</sub></sup> | Recent Developments in Large-Scale Tie-Point Matching  <br> <sup><sub>*Wilfried Hartmann, Michal Havlena, Konrad Schindler*</sub></sup>  | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271615002063)
| 2014 | PHOR | State of the Art in High Density Image Matching   <br> <sup><sub>*Fabio Remondino, Maria Grazia Spera, Erica Nocerino, Fabio Menna, Francesco Nex*</sub></sup>  | [Paper](https://onlinelibrary.wiley.com/doi/abs/10.1111/phor.12063)
| 2012 | PHOR | Development and Status of Image Matching in Photogrammetry  <br> <sup><sub>*Armin Gruen*</sub></sup>  | [Paper](https://onlinelibrary.wiley.com/doi/full/10.1111/j.1477-9730.2011.00671.x)
| :triangular_flag_on_post: | `Semantic` |  | 
| 2022 | GRSM | Deep Learning for Unmanned Aerial Vehicle-Based Object Detection and Tracking: A survey <br> <sub><sup>*Xin Wu; Wei Li; Danfeng Hong; Ran Tao; Qian Du*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/9604009)



<sup><sub>*This table shows only surveys published in top remote sensing journals.</sub></sup>   
<sup><sub>*PERS: Photogrammetric Engineering and Remote Sensing; ISPRS JPRS: International Society for Photogrammetry and Remote Sensing Journal of Photogrammetry and Remote Sensing; RS: Remote Sensing; IJRS: International Journal of Remote Sensing; RSE: Remote Sensing of Environment; GISRS: GIScience & Remote Sensing; PHOR: The Photogrammetric Record; GRSM: IEEE Geoscience and Remote Sensing Magazine.</sub></sup>


### 2. Camera Calibration

- [**Awesome-Deep-Camera-Calibration**](https://github.com/KangLiao929/Awesome-Deep-Camera-Calibration)
- [awesome-image-rectification](https://github.com/bchao1/awesome-image-rectification/tree/master)


| **Year** | **Pub.** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| 2023 | arXiv | Deep Learning for Camera Calibration and Beyond: A Survey   <br> <sub><sup>*Kang Liao, Lang Nie, Shujuan Huang, Chunyu Lin, Jing Zhang, Yao Zhao, Moncef Gabbouj, Dacheng Tao*</sup></sub> | [Paper](https://arxiv.org/abs/2303.10559)/[Proj](https://github.com/KangLiao929/Awesome-Deep-Camera-Calibration)
| 2023 | TIP | Model-aware Pre-training for Radial Distortion Rectification   <br> <sub><sup>*Wendi Wang; Hao Feng; Wengang Zhou; Zhaokang Liao; Houqiang Li*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/10285626)
| 2023 | TIP | SIR: Self-Supervised Image Rectification via Seeing the Same Scene From Multiple Different Lenses   <br> <sub><sup>*Jinlong Fan; Jing Zhang; Dacheng Tao*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/10012683)/[Code](https://github.com/loong8888/SIR)
| 2023 | TCSVT | DaFIR: Distortion-aware Representation Learning for Fisheye Image Rectification   <br> <sub><sup>*Zhaokang Liao; Wengang Zhou; Houqiang Li*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/10251977)/[Code](https://github.com/lzk9508/DaFIR)
| 2023 | ICCV | Innovating Real Fisheye Image Correction with Dual Diffusion Architecture   <br> <sub><sup>*Shangrong Yang, Chunyu Lin, Kang Liao, Yao Zhao*</sup></sub> | [Paper](https://openaccess.thecvf.com/content/ICCV2023/html/Yang_Innovating_Real_Fisheye_Image_Correction_with_Dual_Diffusion_Architecture_ICCV_2023_paper.html)
| 2023 | ICCV | DarSwin: Distortion Aware Radial Swin Transformer  <br> <sub><sup>*Akshaya Athwale, Arman Afrasiyabi, Justin Lagüe, Ichrak Shili, Ola Ahmad, Jean-François Lalonde*</sup></sub> | [Paper](https://openaccess.thecvf.com/content/ICCV2023/html/Athwale_DarSwin_Distortion_Aware_Radial_Swin_Transformer_ICCV_2023_paper.html)/[Code](https://lvsn.github.io/darswin/)
| 2023 | ICCV | Deep Geometry-Aware Camera Self-Calibration from Video  <br> <sub><sup>*Annika Hagemann, Moritz Knorr, Christoph Stiller*</sup></sub> | [Paper](https://openaccess.thecvf.com/content/ICCV2023/html/Hagemann_Deep_Geometry-Aware_Camera_Self-Calibration_from_Video_ICCV_2023_paper.html)/[Code](https://github.com/boschresearch/droidcalib)
| 2023 | CVPR | Wide-Angle Rectification via Content-Aware Conformal Mapping   <br> <sub><sup>*Qi Zhang, Hongdong Li, Qing Wang*</sup></sub> | [Paper](https://openaccess.thecvf.com/content/CVPR2023/html/Zhang_Wide-Angle_Rectification_via_Content-Aware_Conformal_Mapping_CVPR_2023_paper.html)
| 2022 | ECCV | Rethinking Generic Camera Models for Deep Single Image Camera Calibration to Recover Rotation and Fisheye Distortion   <br> <sub><sup>*Nobuhiko Wakai, Satoshi Sato, Yasunori Ishii & Takayoshi Yamashita*</sup></sub> | [Paper](https://link.springer.com/chapter/10.1007/978-3-031-19797-0_39)
| 2022 | IJCV | Wide-Angle Image Rectification: A Survey    <br> <sub><sup>*Jinlong Fan, Jing Zhang, Stephen J. Maybank & Dacheng Tao*</sup></sub> | [Paper](https://link.springer.com/article/10.1007/s11263-021-01562-9)
| 2022 | TCSVT | Revisiting Radial Distortion Rectification in Polar-Coordinates: A New and Efficient Learning Perspective   <br> <sub><sup>*Keyao Zhao; Chunyu Lin; Kang Liao; Shangrong Yang; Yao Zhao*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/9567670)
| 2022 | RAL | Learning-Based Distortion Correction and Feature Detection for High Precision and Robust Camera Calibration   <br> <sub><sup>*Yesheng Zhang; Xu Zhao; Dahong Qian*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/9834080)
| 2021 | ICCV | Towards Complete Scene and Regular Shape for Distortion Rectification by Curve-Aware Extrapolation  <br> <sub><sup>*Kang Liao, Chunyu Lin, Yunchao Wei, Feng Li, Shangrong Yang, Yao Zhao*</sup></sub> | [Paper](https://openaccess.thecvf.com/content/ICCV2021/html/Liao_Towards_Complete_Scene_and_Regular_Shape_for_Distortion_Rectification_by_ICCV_2021_paper.html)
| 2021 | ICCV | Multi-Level Curriculum for Training a Distortion-Aware Barrel Distortion Rectification Model  <br> <sub><sup>*Kang Liao, Chunyu Lin, Lixin Liao, Yao Zhao, Weiyao Lin*</sup></sub> | [Paper](https://openaccess.thecvf.com/content/ICCV2021/html/Liao_Multi-Level_Curriculum_for_Training_a_Distortion-Aware_Barrel_Distortion_Rectification_Model_ICCV_2021_paper.html)
| 2021 | CVPR | Progressively Complementary Network for Fisheye Image Rectification Using Appearance Flow  <br> <sub><sup>*Shangrong Yang, Chunyu Lin, Kang Liao, Chunjie Zhang, Yao Zhao*</sup></sub> | [Paper](https://openaccess.thecvf.com/content/CVPR2021/html/Yang_Progressively_Complementary_Network_for_Fisheye_Image_Rectification_Using_Appearance_Flow_CVPR_2021_paper.html)/[Code](https://github.com/uof1745-cmd/PCN)
| 2021 | TIP | A Deep Ordinal Distortion Estimation Approach for Distortion Rectification <br> <sub><sup>*Kang Liao; Chunyu Lin; Yao Zhao*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/9366359)
| 2020 | ICASSP | Self-Supervised Deep Learning for Fisheye Image Rectification   <br> <sub><sup>*Chun-Hao Chao; Pin-Lun Hsu; Hung-Yi Lee; Yu-Chiang Frank Wang*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/9054191)
| 2019 | CVPR | Learning Structure-And-Motion-Aware Rolling Shutter Correction	  <br> <sub><sup>*Bingbing Zhuang, Quoc-HuyTran, PanJi, Loong-Fah Cheong, Manmohan Chandraker*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_CVPR_2019/html/Zhuang_Learning_Structure-And-Motion-Aware_Rolling_Shutter_Correction_CVPR_2019_paper.html)
| 2019 | CVPR | Blind Geometric Distortion Correction on Images Through Deep Learning   <br> <sub><sup>*Xiaoyu Li, Bo Zhang, Pedro V. Sander, Jing Liao*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_CVPR_2019/html/Li_Blind_Geometric_Distortion_Correction_on_Images_Through_Deep_Learning_CVPR_2019_paper.html)/[Code](https://github.com/xiaoyu258/GeoProj)
| 2019 | CVPR | Learning to calibrate straight lines for fisheye image rectification   <br> <sub><sup>*Xue, Zhucun and Xue, Nan and Xia, Gui-Song and Shen, Weiming*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_CVPR_2019/html/Xue_Learning_to_Calibrate_Straight_Lines_for_Fisheye_Image_Rectification_CVPR_2019_paper.html)
| 2018 | ECCV | Fisheyerecnet: A multi-context collaborative deep network for fisheye image rectification   <br> <sub><sup>*Yin, Xiaoqing and Wang, Xinchao and Yu, Jun and Zhang, Maojun and Fua, Pascal and Tao, Dacheng*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_ECCV_2018/html/Xiaoqing_Yin_FishEyeRecNet_A_Multi-Context_ECCV_2018_paper.html)
| 2016 | ACCV | Radial lens distortion correction using convolutional neural networks trained with synthesized images   <br> <sub><sup>*Rong, Jiangpeng and Huang, Shiyao and Shang, Zeyu and Ying, Xianghua*</sup></sub> | [Paper](https://link.springer.com/chapter/10.1007/978-3-319-54187-7_3)
| 2015 | CVPR | Line-based multi-label energy optimization for fisheye image rectification and calibration  <br> <sub><sup>*Zhang, Mi and Yao, Jian and Xia, Menghan and Li, Kai and Zhang, Yi and Liu, Yaping*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_cvpr_2015/html/Zhang_Line-Based_Multi-Label_Energy_2015_CVPR_paper.html)
| 2015 | ISPRS JPRS | Generating 3D hyperspectral information with lightweight UAV snapshot cameras for vegetation monitoring: From camera calibration to quality assurance  <br> <sub><sup>*Aasen, Helge and Burkart, Andreas and Bolten, Andreas and Bareth, Georg*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271615001938)
| 2013 | IROS | AprilCal: Assisted and repeatable camera calibration <br> <sub><sup>*Richardson, Andrew and Strom, Johannes and Olson, Edwin*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/6696595)
| 2010 | PAMI | Equidistant fish-eye calibration and rectification by vanishing point extraction <br> <sub><sup>*Hughes, Ciaran and Denny, Patrick and Glavin, Martin and Jones, Edward*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/5557882)
| 2008 | CVPR | On benchmarking camera calibration and multi-view stereo for high resolution imagery <br> <sub><sup>*Strecha, Christoph and Von Hansen, Wolfgang and Van Gool, Luc and Fua, Pascal and Thoennessen, Ulrich*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/4587706)
| 2006 | PAMI | A generic camera model and calibration method for conventional, wide-angle, and fish-eye lenses  <br> <sub><sup>*Kannala, Juho and Brandt, Sami S*</sup></sub> | [Paper](https://ieeexplore.ieee.org/document/1642666)
| 2000 | PAMI | A flexible new technique for camera calibration  <br> <sub><sup>*Zhang, Zhengyou*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/888718)





### 3. Combined field of view


58 - 65
49，22


### 4. Low-altitude UAV image matching

Multi-view image matching 
66- 81
29， 39


Matching with non-UAV images
83 - 87 
67， 70


88-92 

### 5. Low-altitude automatic aerial triangulation

93-97
20 

structure from motion: 98-101 
Image orientation: 102 - 106
SfM for Rolling Shutter Cameras (RSC): 107 - 110 


### 6. Dense reconstruction

15 
28,69 111-114
115-125



### 7. Image stitching

126-130 
Ortho-rectification based image stitching: 102 133 131
Transformation based image stitching: 134 - 142, 132, 66, 143, 144



### 8. Multi-sensor data registration
145-147
Multi-band image registration: 148-152 
 
Registration of LiDAR and optical images: 153-154


### 9. High-performance data processing

102， 155-161


## Dataset and Tools 









## Citation

Please cite our paper if you find the work useful:

```
@article{fan2023csu,
  title={Mini-Unmanned Aerial Vehicle-Based Remote Sensing: Techniques, Applications, and Prospects},
  author={Tian-Zhu Xiang, Gui-Song Xia, Liangpei Zhang},
  journal={IEEE Geoscience and Remote Sensing Magazine},
  pages={29 - 63},
  volume={7},
  number={3},
  doi={10.1109/MGRS.2019.2918840},  
  year={2019}
}
```

