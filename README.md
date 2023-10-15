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

We hope this paper will provide remote-sensing researchers an overall picture of recent UAV-based remote sensing developments and help guide further research on this topic.



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





### 3. Combined field of view




### 4. Low-altitude UAV image matching



### 5. Low-altitude automatic aerial triangulation


### 6. Dense reconstruction


### 7. Image stitching


### 8. Multi-sensor data registration


### 9. High-performance data processing




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

