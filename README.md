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
- [Dataset & Tools](#Dataset-and-Tools) 
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
| 2015  | JCR | Coastal and Environmental Remote Sensing from Unmanned Aerial Vehicles: An Overview  <br> <sup><sub>*Victor V. Klemas*</sub></sup>  | [Paper](https://meridian.allenpress.com/jcr/article-abstract/31/5/1260/144921/Coastal-and-Environmental-Remote-Sensing-from)
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
- [Awesome-Image-Distortion-Correction](https://github.com/subeeshvasu/Awesome-Image-Distortion-Correction)
- [Awesome-Image-Rectification](https://github.com/bchao1/awesome-image-rectification/tree/master)


| **Year** | **Pub.** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| 2023 | arXiv | Deep Learning for Camera Calibration and Beyond: A Survey   <br> <sub><sup>*Kang Liao, Lang Nie, Shujuan Huang, Chunyu Lin, Jing Zhang, Yao Zhao, Moncef Gabbouj, Dacheng Tao*</sup></sub> | [Paper](https://arxiv.org/abs/2303.10559)/[Proj](https://github.com/KangLiao929/Awesome-Deep-Camera-Calibration)
| 2023 | ICCV | Innovating Real Fisheye Image Correction with Dual Diffusion Architecture   <br> <sub><sup>*Shangrong Yang, Chunyu Lin, Kang Liao, Yao Zhao*</sup></sub> | [Paper](https://openaccess.thecvf.com/content/ICCV2023/html/Yang_Innovating_Real_Fisheye_Image_Correction_with_Dual_Diffusion_Architecture_ICCV_2023_paper.html)
| 2023 | ICCV | DarSwin: Distortion Aware Radial Swin Transformer  <br> <sub><sup>*Akshaya Athwale, Arman Afrasiyabi, Justin Lagüe, Ichrak Shili, Ola Ahmad, Jean-François Lalonde*</sup></sub> | [Paper](https://openaccess.thecvf.com/content/ICCV2023/html/Athwale_DarSwin_Distortion_Aware_Radial_Swin_Transformer_ICCV_2023_paper.html)/[Code](https://lvsn.github.io/darswin/)
| 2023 | ICCV | Deep Geometry-Aware Camera Self-Calibration from Video  <br> <sub><sup>*Annika Hagemann, Moritz Knorr, Christoph Stiller*</sup></sub> | [Paper](https://openaccess.thecvf.com/content/ICCV2023/html/Hagemann_Deep_Geometry-Aware_Camera_Self-Calibration_from_Video_ICCV_2023_paper.html)/[Code](https://github.com/boschresearch/droidcalib)
| 2023 | CVPR | Wide-Angle Rectification via Content-Aware Conformal Mapping   <br> <sub><sup>*Qi Zhang, Hongdong Li, Qing Wang*</sup></sub> | [Paper](https://openaccess.thecvf.com/content/CVPR2023/html/Zhang_Wide-Angle_Rectification_via_Content-Aware_Conformal_Mapping_CVPR_2023_paper.html)
| 2023 | TIP | Model-aware Pre-training for Radial Distortion Rectification   <br> <sub><sup>*Wendi Wang; Hao Feng; Wengang Zhou; Zhaokang Liao; Houqiang Li*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/10285626)
| 2023 | TIP | SIR: Self-Supervised Image Rectification via Seeing the Same Scene From Multiple Different Lenses   <br> <sub><sup>*Jinlong Fan; Jing Zhang; Dacheng Tao*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/10012683)/[Code](https://github.com/loong8888/SIR)
| 2023 | TCSVT | DaFIR: Distortion-aware Representation Learning for Fisheye Image Rectification   <br> <sub><sup>*Zhaokang Liao; Wengang Zhou; Houqiang Li*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/10251977)/[Code](https://github.com/lzk9508/DaFIR)
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
| 2015 | CVPR | Line-based multi-label energy optimization for fisheye image rectification and calibration  <br> <sub><sup>*Zhang, Mi and Yao, Jian and Xia, Menghan and Li, Kai and Zhang, Yi and Liu, Yaping*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_cvpr_2015/html/Zhang_Line-Based_Multi-Label_Energy_2015_CVPR_paper.html)/[Code](http://cvrs.whu.edu.cn/projects/FIRC/)
| 2015 | ISPRS JPRS | Generating 3D hyperspectral information with lightweight UAV snapshot cameras for vegetation monitoring: From camera calibration to quality assurance  <br> <sub><sup>*Aasen, Helge and Burkart, Andreas and Bolten, Andreas and Bareth, Georg*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271615001938)
| 2014 | IPOL | Automatic Lens Distortion Correction Using One-Parameter Division Models  <br> <sub><sup>*Miguel Alemán-Flores, Luis Alvarez, Luis Gomez, Daniel Santana-Cedrés*</sup></sub> | [Paper](https://www.ipol.im/pub/art/2014/106/)/[Code](https://www.ipol.im/pub/art/2014/106/)
| 2013 | IROS | AprilCal: Assisted and repeatable camera calibration <br> <sub><sup>*Richardson, Andrew and Strom, Johannes and Olson, Edwin*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/6696595)
| 2010 | PAMI | Equidistant fish-eye calibration and rectification by vanishing point extraction <br> <sub><sup>*Hughes, Ciaran and Denny, Patrick and Glavin, Martin and Jones, Edward*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/5557882)
| 2008 | CVPR | On benchmarking camera calibration and multi-view stereo for high resolution imagery <br> <sub><sup>*Strecha, Christoph and Von Hansen, Wolfgang and Van Gool, Luc and Fua, Pascal and Thoennessen, Ulrich*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/4587706)
| 2006 | PAMI | A generic camera model and calibration method for conventional, wide-angle, and fish-eye lenses  <br> <sub><sup>*Kannala, Juho and Brandt, Sami S*</sup></sub> | [Paper](https://ieeexplore.ieee.org/document/1642666)
| 2000 | PAMI | A flexible new technique for camera calibration  <br> <sub><sup>*Zhang, Zhengyou*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/888718)




### 3. Combined field of view

- Combined field of view to expand coverage
- Aerial path planning for optimal area coverage

| **Year** | **Pub.** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| 2023 | JSTARS | A Review on Viewpoints and Path Planning for UAV-Based 3-D Reconstruction   <br> <sub><sup>*Mehdi Maboudi; MohammadReza Homaei; Soohwan Song; Shirin Malihi, et al*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/10124957)
| 2022 | <sub><sup>Auton Robot</sup></sub> | Cooperative multi-UAV coverage mission planning platform for remote sensing applications  <br> <sub><sup>*Savvas D. Apostolidis, Pavlos Ch. Kapoutsis, Athanasios Ch. Kapoutsis & Elias B. Kosmatopoulos*</sup></sub> | [Paper](https://link.springer.com/article/10.1007/s10514-021-10028-3)/[Code](https://github.com/savvas-ap/mCPP-optimized-DARP)
| 2021 | ToG | Continuous aerial path planning for 3D urban scene reconstruction  <br> <sub><sup>*Han Zhang, Yucong Yao, Ke Xie, Chi-Wing Fu, Hao Zhang, Hui Huang*</sup></sub> | [Paper](https://dl.acm.org/doi/abs/10.1145/3478513.3480483)
| 2021 | TRO | View Path Planning via Online Multiview Stereo for 3-D Modeling of Large-Scale Structures  <br> <sub><sup>*Soohwan Song; Daekyum Kim; Sunghee Choi*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/9450826)
| 2020 | ToG | Offsite aerial path planning for efficient urban scene reconstruction   <br> <sub><sup>*Xiaohui Zhou, Ke Xie, Kai Huang, Yilin Liu, Yang Zhou, Minglun Gong, Hui Huang*</sup></sub> | [Paper](https://dl.acm.org/doi/abs/10.1145/3414685.3417791)
| 2018 | ToG | Aerial Path Planning for Urban Scene Reconstruction: A Continuous Optimization Method and Benchmark   <br> <sub><sup>*Neil Smith, Nils Moehrle, Michael Goesele, Wolfgang Heidrich*</sup></sub> | [Paper](https://dl.acm.org/doi/10.1145/3272127.3275010) 
| 2018 | Sensors | Multi-camera imaging system for UAV photogrammetry   <br> <sub><sup>*Wierzbicki, Damian*</sup></sub> | [Paper](https://www.mdpi.com/1424-8220/18/8/2433)
| 2018 | TSG | Multi-UAV Pre-Positioning and Routing for Power Network Damage Assessment  <br> <sub><sup>*Gino J. Lim; Seonjin Kim; Jaeyoung Cho; Yibin Gong; Amin Khodaei*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/7778146)
| 2015 | Sensors | Multi-UAV Routing for Area Coverage and Remote Sensing with Minimum Time  <br> <sub><sup>*Gustavo S. C. Avellar, Guilherme A. S. Pereira, Luciano C. A. Pimenta and Paulo Iscold*</sup></sub> | [Paper](https://www.mdpi.com/1424-8220/15/11/27783)
| 2013 | IJARS | A solution to cooperative area coverage surveillance for a swarm of MAVs  <br> <sub><sup>*Zheng-Jie, Wang and Wei, Li*</sup></sub> | [Paper](https://journals.sagepub.com/doi/full/10.5772/56801)
| 2012 | ISPRSC | UAV borne low altitude photogrammetry system   <br> <sub><sup>*Z. Lin, G. Su, and F. Xie*</sup></sub> | [Paper](https://isprs-archives.copernicus.org/articles/XXXIX-B1/415/2012/)




### 4. Low-altitude UAV image matching

:small_orange_diamond: **Multi-view image matching** 

- [Awesome-Image-Matching](https://github.com/ericzzj1989/Awesome-Image-Matching)
- [Awesome-Computational-Photography](https://github.com/visionxiang/awesome-computational-photography/blob/main/README.md#Image-Matching)


| **Year** | **Pub.** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| 2022 | <sup><sub>ISPRS JPRS</sub></sup> | Leveraging vocabulary tree for simultaneous match pair selection and guided feature matching of UAV images   <br> <sub><sup>*San Jiang, Wanshou Jiang, Bingxuan Guo*</sup></sub>  | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271622000727)
| 2022 | AAAI |  Guide Local Feature Matching by Overlap Estimation   <br> <sub><sup>*Ying Chen, Dihe Huang, et al*</sup></sub> | [Paper](https://aaai-2022.virtualchair.net/poster_aaai7556)/[Code](https://github.com/AbyssGaze/OETR)
| 2021 | IJCV | Image Matching from Handcrafted to Deep Features: A Survey  <br> <sub><sup>*Jiayi Ma, Xingyu Jiang, Aoxiang Fan, Junjun Jiang & Junchi Yan*</sup></sub> | [Paper](https://link.springer.com/article/10.1007/s11263-020-01359-2)
| 2020 | IJCV | Image Matching across Wide Baselines: From Paper to Practice <br> <sub><sup>*Yuhe Jin and Dmytro Mishkin and Anastasiia Mishchuk and Jiri Matas and Pascal Fua and Kwang Moo Yi and Eduard Trulls*</sup></sub> | [Paper](https://link.springer.com/article/10.1007/s11263-020-01385-0)/[Code](https://github.com/ubc-vision/image-matching-benchmark)
| 2019 | <sup><sub>ISPRS JPRS</sub></sup> | LAM: Locality affine-invariant feature matching  <br> <sub><sup>*Jiayuan Li, Qingwu Hu, Mingyao Ai*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271619301285)
| 2018 | ECCV | Geodesc: Learning local descriptors by integrating geometry constraints  <br> <sub><sup>*Z. Luo, T. Shen, L. Zhou, S. Zhu, R. Zhang, Y. Yao, T. Fang, and L. Quan*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_ECCV_2018/html/Zixin_Luo_Learning_Local_Descriptors_ECCV_2018_paper.html)/[Code](https://github.com/lzx551402/geodesc)
| 2018 | JARS | Unmanned aerial vehicle oblique image registration using an ASIFT-based matching method  <br> <sub><sup>*Wang, Chengyi and Chen, Jingbo and Chen, Jiansheng and Yue, Anzhi and He, Dongxu and Huang, Qingqing and Zhang, Yi*</sup></sub> | [Paper](https://www.spiedigitallibrary.org/journals/journal-of-applied-remote-sensing/volume-12/issue-2/025002/Unmanned-aerial-vehicle-oblique-image-registration-using-an-ASIFT-based/10.1117/1.JRS.12.025002.short?SSO=1)
| 2018 | IJRS | Registrating oblique images by integrating affine and scale-invariant features  <br> <sub><sup>*Yu, Mei and Yang, Huachao and Deng, Kazhong and Yuan, Kai*</sup></sub> | [Paper](https://www.tandfonline.com/doi/abs/10.1080/01431161.2017.1362129)
| 2018 | <sub><sup>ISPRS JPRS</sup></sub> | Hierarchical motion consistency constraint for efficient geometrical verification in UAV stereo image matching  <br> <sub><sup>*Jiang, San and Jiang, Wanshou*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271618301722)
| 2017 | ICCV | Progressive Large Scale-Invariant Image Matching in Scale Space  <br> <sub><sup>*Lei Zhou, Siyu Zhu, Tianwei Shen, Jinglu Wang, Tian Fang, Long Quan*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_iccv_2017/html/Zhou_Progressive_Large_Scale-Invariant_ICCV_2017_paper.html)
| 2017 | ICCV | Learning discriminative and transformation covariant local feature detectors  <br> <sub><sup>*X. Zhang, F. X. Yu, S. Karaman, and S.-F. Chang*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_cvpr_2017/html/Zhang_Learning_Discriminative_and_CVPR_2017_paper.html)/[Code](https://github.com/ColumbiaDVMM/Transform_Covariant_Detector)
| 2017 | ICCV | Learning spread-out local feature descriptors <br> <sub><sup>*X. Zhang, F. X. Yu, S. Kumar, and S.-F. Chang*</sup></sub> | [Paper](https://arxiv.org/abs/1708.06320)/[Code](https://github.com/ColumbiaDVMM/hardnet)
| 2017 | CVPR | HPatches: A benchmark and evaluation of handcrafted and learned local descriptors  <br> <sub><sup>*Balntas, Vassileios and Lenc, Karel and Vedaldi, Andrea and Mikolajczyk, Krystian*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_cvpr_2017/html/Balntas_HPatches_A_Benchmark_CVPR_2017_paper.html)/[Code](https://hpatches.github.io/)
| 2017 | RS | On-board GNSS/IMU assisted feature extraction and matching for oblique UAV images  <br> <sub><sup>*S. Jiang and W. Jiang*</sup></sub> | [Paper](https://www.mdpi.com/2072-4292/9/8/813)
| 2016 | CVPR | Learning to match aerial images with deep attentive architectures   <br> <sub><sup>*H. Altwaijry, E. Trulls, J. Hays, P. Fua, and S. Belongie*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_cvpr_2016/html/Altwaijry_Learning_to_Match_CVPR_2016_paper.html)
| 2015 | CVPR | TILDE: A Temporally Invariant Learned DEtector <br> <sub><sup>*Yannick Verdie, Kwang Yi, Pascal Fua, Vincent Lepetit*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_cvpr_2015/html/Verdie_TILDE_A_Temporally_2015_CVPR_paper.html)/[Code](https://github.com/vcg-uvic/TILDE)
| 2015 | PERS | Reliable spatial relationship constrained feature point matching of oblique aerial images  <br> <sub><sup>*Hu, Han and Zhu, Qing and Du, Zhiqiang and Zhang, Yeting and Ding, Yulin*</sup></sub> | [Paper](https://www.ingentaconnect.com/content/asprs/pers/2015/00000081/00000001/art00003)
| 2015 | RS | A robust photogrammetric processing method of low-altitude UAV images  <br> <sub><sup>*Ai, Mingyao and Hu, Qingwu and Li, Jiayuan and Wang, Ming and Yuan, Hui and Wang, Shaohua*</sup></sub> | [Paper](https://www.mdpi.com/2072-4292/7/3/2302)
| 2014 | <sub><sup>ISPRS JPRS</sup></sub> | L2-SIFT: SIFT feature extraction and matching for large images in large-scale aerial photogrammetry  <br> <sub><sup>*Sun, Yanbiao and Zhao, Liang and Huang, Shoudong and Yan, Lei and Dissanayake, Gamini*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S092427161400029X)
| 2012 | PhotoRec | Development and status of image matching in photogrammetry   <br> <sub><sup>*Armin Gruen*</sup></sub> | [Paper](https://onlinelibrary.wiley.com/doi/full/10.1111/j.1477-9730.2011.00671.x)



:small_orange_diamond: **Matching with non-UAV images**

| **Year** | **Pub.** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| 2022 | RS | Multiview Image Matching of Optical Satellite and UAV Based on a Joint Description Neural Network   <br> <sub><sup>*Chuan Xu, Chang Liu, Hongli Li, Zhiwei Ye, Haigang Sui and Wei Yang*</sup></sub> | [Paper](https://www.mdpi.com/2072-4292/14/4/838)
| 2021 | RS | A Practical Cross-View Image Matching Method between UAV and Satellite for UAV-Based Geo-Localization  <br> <sub><sup>*Lirong Ding, Ji Zhou, Lingxuan Meng and Zhiyong Long*</sup></sub> | [Paper](https://www.mdpi.com/2072-4292/13/1/47)
| 2017 | RS | Automatic UAV image geo-registration by matching UAV images to georeferenced image data   <br> <sub><sup>*Xiangyu Zhuo, Tobias Koch, Franz Kurz, Friedrich Fraundorfer and Peter Reinartz*</sup></sub>  | [Paper](https://www.mdpi.com/2072-4292/9/4/376)
| 2016 | <sup><sub>ISPRS JPRS</sub></sup> | Illumination-invariant image matching for autonomous UAV localisation based on optical sensing  <br> <sub><sup>*Xue Wan, Jianguo Liu, Hongshi Yan, Gareth L.K. Morgan*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271616301113)
| :triangular_flag_on_post: | G2A | | | 
| 2023 | AAAI | Cross-View Geo-Localization via Learning Disentangled Geometric Layout Correspondence <br> <sub><sup>*Xiaohan Zhang, Xingyu Li, Waqas Sultani, Yi Zhou, Safwan Wshah*</sup></sub> | [Paper](https://ojs.aaai.org/index.php/AAAI/article/view/25457)
| 2019 | ICCV | Bridging the Domain Gap for Ground-to-Aerial Image Matching  <br> <sub><sup>*Krishna Regmi, Mubarak Shah*</sup></sub> | [Paper](https://arxiv.org/abs/1904.11045)/[Code](https://github.com/kregmi/cross-view-image-matching)
| 2019 | ICCV | Ground-to-Aerial Image Geo-Localization With a Hard Exemplar Reweighting Triplet Loss  <br> <sub><sup>*Sudong Cai, Yulan Guo, Salman Khan, Jiwei Hu, Gongjian Wen*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_ICCV_2019/html/Cai_Ground-to-Aerial_Image_Geo-Localization_With_a_Hard_Exemplar_Reweighting_Triplet_Loss_ICCV_2019_paper.html)
| 2018 | CVPR | CVM-net: Cross-view matching network for image-based ground-to-aerial geo-localization  <br> <sub><sup>*Sixing Hu, Mengdan Feng, Rang MH Nguyen, and Gim Hee Lee*</sup></sub> | [Paper](http://openaccess.thecvf.com/content_cvpr_2018/html/Hu_CVM-Net_Cross-View_Matching_CVPR_2018_paper.html)/[Code](https://github.com/david-husx/crossview_localisation)
| 2016 | CVPR | Regularity-driven building facade matching between aerial and street views  <br> <sub><sup>*M. Wolff, R. T. Collins, and Y. Liu*</sup></sub> | [Paper](https://www.cv-foundation.org/openaccess/content_cvpr_2016/html/Wolff_Regularity-Driven_Facade_Matching_CVPR_2016_paper.html)
| 2014 | 3DV | Accurate geo-registration by ground-to-aerial image matching   <br> <sub><sup>*S. Qi, C. Wu, B. Curless, Y. Furukawa, C. Hernandez, and S. M. Seitz*</sup></sub> | [Paper](https://ieeexplore.ieee.org/document/7035866)




### 5. Low-altitude automatic aerial triangulation

:small_orange_diamond: **Structure from motion** 

| **Year** | **Pub.** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- | 
| 2020 | ECCV | DeepSFM: Structure From Motion Via Deep Bundle Adjustment   <br> <sub><sup>*Xingkui Wei, Yinda Zhang, Zhuwen Li, Yanwei Fu, Xiangyang Xue*</sup></sub> | [Paper](https://arxiv.org/abs/1912.09697)/[Code](https://weixk2015.github.io/DeepSFM/)
| 2020 | <sup><sub>ISPRS JPRS</sub></sup> | Efficient structure from motion for large-scale UAV images: A review and a comparison of SfM tools  <br> <sub><sup>*San Jiang, Cheng Jiang, Wanshou Jiang*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271620301131)
| 2019 | CFR | Structure from Motion Photogrammetry in Forestry: a Review     <br> <sub><sup>*Jakob Iglhaut, Carlos Cabo, Stefano Puliti, Livia Piermattei, James O’Connor & Jacqueline Rosette*</sup></sub>  | [Paper](https://link.springer.com/article/10.1007/s40725-019-00094-3)
| 2017 | ICCV | Parallel Structure from Motion from Local Increment to Global Averaging   <br> <sub><sup>*Siyu Zhu, Tianwei Shen, Lei Zhou, Runze Zhang, Jinglu Wang, Tian Fang, Long Quan*</sup></sub> | [Paper](https://arxiv.org/abs/1702.08601)
| 2017 | ICCV | Distributed Very Large Scale Bundle Adjustment by Global Camera Consensus  <br> <sub><sup>*Runze Zhang, Siyu Zhu, Tian Fang, Long Quan*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_iccv_2017/html/Zhang_Distributed_Very_Large_ICCV_2017_paper.html)
| 2017 | CVPR | HSfM: Hybrid Structure-from-Motion   <br> <sub><sup>*Hainan Cui, Xiang Gao, Shuhan Shen, Zhanyi Hu*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_cvpr_2017/html/Cui_HSfM_Hybrid_Structure-from-Motion_CVPR_2017_paper.html)/[Code](https://github.com/sweeneychris/TheiaSfM/blob/master/src/theia/sfm/hybrid_reconstruction_estimator.h)
| 2017 | CVPR | Unsupervised learning of depth and ego-motion from video     <br> <sub><sup>*Tinghui Zhou, Matthew Brown, Noah Snavely, David G. Lowe*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_cvpr_2017/html/Zhou_Unsupervised_Learning_of_CVPR_2017_paper.html)/[Code](https://github.com/ClementPinard/SfmLearner-Pytorch)
| 2017 | ActaNum |  A survey of structure from motion  <br> <sub><sup>*Onur Özyeşil, Vladislav Voroninski, Ronen Basri and Amit Singer*</sup></sub> | [Paper](https://www.cambridge.org/core/journals/acta-numerica/article/abs/survey-of-structure-from-motion/C4B2E7BB10BC2C11AF71BC80B584D378)
| 2016 | CVPR | Structure-from-Motion Revisited  <br> <sub><sup>*Schonberger, Johannes Lutz and Frahm, Jan-Michael*</sup></sub> | [Paper](https://www.cv-foundation.org/openaccess/content_cvpr_2016/html/Schonberger_Structure-From-Motion_Revisited_CVPR_2016_paper.html)/[Code](https://github.com/colmap/colmap)
| 2015 | ICCV | PoseNet: A Convolutional Network for Real-Time 6-DOF Camera Relocalization   <br> <sub><sup>*Alex Kendall, Matthew Grimes, Roberto Cipolla*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_iccv_2015/html/Kendall_PoseNet_A_Convolutional_ICCV_2015_paper.html)/[Code](https://github.com/alexgkendall/caffe-posenet)
| 2014 | ECCV | Robust global translations with 1DSFM     <br> <sub><sup>*Kyle Wilson & Noah Snavely*</sup></sub> | [Paper](https://link.springer.com/chapter/10.1007/978-3-319-10578-9_5)/[Code](https://github.com/wilsonkl/SfM_Init)
| 2012 | CVPR | Semantic structure from motion with points, regions, and objects   <br> <sub><sup>*Sid Yingze Bao; Mohit Bagra; Yu-Wei Chao; Silvio Savarese*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/6247992)
| 2012 | Geom | ‘Structure-from-Motion’ photogrammetry: A low-cost, effective tool for geoscience applications  <br> <sub><sup>*M.J. Westoby, J. Brasington, N.F. Glasser, M.J. Hambrey, J.M. Reynolds*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/pii/S0169555X12004217)
| 2011 | PhotoRec | Photogrammetric processing of low-altitude images acquired by unpiloted aerial vehicles  <br> <sub><sup>*Yongjun Zhang, Jinxin Xiong, Lijuan Hao*</sup></sub> | [Paper](https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1477-9730.2011.00641.x)



:small_orange_diamond: **Rolling-shutter SfM** 

| **Year** | **Pub.** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- | 
| 2023 | CVPR | Revisiting Rolling Shutter Bundle Adjustment: Toward Accurate and Fast Solution   <br> <sub><sup>*Bangyan Liao, Delin Qu, Yifei Xue, Huiqing Zhang, Yizhen Lao*</sup></sub> | [Paper](https://openaccess.thecvf.com/content/CVPR2023/html/Liao_Revisiting_Rolling_Shutter_Bundle_Adjustment_Toward_Accurate_and_Fast_Solution_CVPR_2023_paper.html)/[Code](https://delinqu.github.io/NW-RSBA/)
| 2023 | RS | Experimental Tests and Simulations on Correction Models for the Rolling Shutter Effect in UAV Photogrammetry  <br> <sub><sup>*Nazarena Bruno and Gianfranco Forlani*</sup></sub> | [Paper](https://www.mdpi.com/2072-4292/15/9/2391)
| 2021 | IJCV | Solving Rolling Shutter 3D Vision Problems using Analogies with Non-rigidity  <br> <sub><sup>*Yizhen Lao, Omar Ait-Aider & Adrien Bartoli*</sup></sub> | [Paper](https://link.springer.com/article/10.1007/s11263-020-01368-1)
| 2019 | PAMI | Accurate 3D Reconstruction from Small Motion Clip for Rolling Shutter Cameras  <br> <sub><sup>*Im, Sunghoon and Ha, Hyowon and Choe, Gyeongmin and Jeon, Hae-Gon and Joo, Kyungdon and Kweon, In So*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/8325527)
| 2019 | CVPR | Learning Structure-And-Motion-Aware Rolling Shutter Correction   <br> <sub><sup>*Bingbing Zhuang, Quoc-Huy Tran, Pan Ji, Loong-Fah Cheong, Manmohan Chandraker*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_CVPR_2019/html/Zhuang_Learning_Structure-And-Motion-Aware_Rolling_Shutter_Correction_CVPR_2019_paper.html)
| 2018 | PRL | Robustified Structure from Motion with rolling-shutter camera using straightness constraint  <br> <sub><sup>*Yizhen Lao, Omar Ait-Aider, Helder Araujo*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0167865518301247)
| 2017 | CVPR | Self-Calibration-Based Approach to Critical Motion Sequences of Rolling-Shutter Structure From Motion <br> <sub><sup>*Eisuke Ito, Takayuki Okatani*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_cvpr_2017/html/Ito_Self-Calibration-Based_Approach_to_CVPR_2017_paper.html)
| 2017 | CVPR | Unrolling the shutter: CNN to correct motion distortions  <br> <sub><sup>*Vijay Rengarajan, Yogesh Balaji, A. N. Rajagopalan*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_cvpr_2017/html/Rengarajan_Unrolling_the_Shutter_CVPR_2017_paper.html)
| 2016 | CVPR | From bows to arrows: Rolling shutter rectification of urban scenes  <br> <sub><sup>*Vijay Rengarajan, Ambasamudram N. Rajagopalan, Rangarajan Aravind*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_cvpr_2016/html/Rengarajan_From_Bows_to_CVPR_2016_paper.html)
| 2015 | ICCV | High quality structure from small motion for rolling shutter cameras  <br> <sub><sup>*Sunghoon Im, Hyowon Ha, Gyeongmin Choe, Hae-Gon Jeon, Kyungdon Joo, In So Kweon*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_iccv_2015/html/Im_High_Quality_Structure_ICCV_2015_paper.html)
| 2013 | ICCV | Street view motion-from structure-from-motion  <br> <sub><sup>*Bryan Klingner, David Martin, James Roseborough*</sup></sub> | [Paper](https://www.cv-foundation.org/openaccess/content_iccv_2013/html/Klingner_Street_View_Motion-from-Structure-from-Motion_2013_ICCV_paper.html)
| 2013 | CVPR | Rolling Shutter Camera Calibration   <br> <sub><sup>*Luc Oth, Paul Furgale, Laurent Kneip, Roland Siegwart*</sup></sub> | [Paper](https://www.cv-foundation.org/openaccess/content_cvpr_2013/html/Oth_Rolling_Shutter_Camera_2013_CVPR_paper.html)
| 2012 | CVPR | Rolling shutter bundle adjustment   <br> <sub><sup>*Johan Hedborg; Per-Erik Forssén; Michael Felsberg; Erik Ringaby*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/6247831)



:small_orange_diamond: **SfM Toolkit** 

| **Name** | **Year** | **Pub**          | 
| :------ | :------: | :----------------------------------------------------------- |  
| [OpenSfM](https://github.com/mapillary/OpenSfM) |  | [Homepage](www.opensfm.org/)
| [ColMap](https://github.com/colmap/colmap) | 2016 | [CVPR](https://www.cv-foundation.org/openaccess/content_cvpr_2016/html/Schonberger_Structure-From-Motion_Revisited_CVPR_2016_paper.html)
| [OpenMVG](https://github.com/openMVG/openMVG) | 2016 | 
| [TheiaSfM](https://github.com/sweeneychris/TheiaSfM) | 2015 | 
| [MVE](https://github.com/simonfuhrmann/mve) | 2014 | [Proceedings](https://diglib.eg.org/handle/10.2312/gch.20141299.011-018)
| [VisualSFM](http://ccwu.me/vsfm/index.html) | 2011 |
| [Bundler](https://github.com/snavely/bundler_sfm) | 2006 | 
| [Ceres Solver](https://github.com/ceres-solver/ceres-solver) | 2023 | [Doc](http://ceres-solver.org/)
| [Regard3D](https://www.regard3d.org/index.php) | 2019 | 
  
  


### 6. Dense reconstruction

- [Awesome MVS](https://github.com/walsvid/Awesome-MVS)
  

| **Year** | **Pub.** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- | 
| 2023 | <sup><sub>ISPRS JPRS</sub></sup> | Deep learning based multi-view stereo matching and 3D scene reconstruction from oblique aerial images <br> <sub><sup>*Jin Liu, Jian Gao, Shunping Ji, Chang Zeng, Shaoyi Zhang, JianYa Gong*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/pii/S0924271623002289)/[Code](http://gpcv.whu.edu.cn/data)
| 2023 | <sup><sub>ISPRS JPRS</sub></sup> | Multiple View Stereo with quadtree-guided priors  <br> <sub><sup>*Elisavet Konstantina Stathopoulou, Roberto Battisti, Dan Cernea, Andreas Georgopoulos, Fabio Remondino*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271622003288)/[Code](https://github.com/3DOM-FBK/openMVS)
| 2023 | TGRS | Select-and-Combine (SAC): A Novel Multi-stereo Depth Fusion Algorithm for Point Cloud Generation via Efficient Local Markov Netlets  <br> <sub><sup>*Mostafa Elhashash; Rongjun Qin*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/10210605)
| 2023 | TGRS | A Hierarchical Deformable Deep Neural Network and an Aerial Image Benchmark Dataset for Surface Multiview Stereo Reconstruction  <br> <sub><sup>*Jiayi Li; Xin Huang; Yujin Feng; Zhen Ji; Shulei Zhang; Dawei Wen*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/10007846)
| 2022 | ECCV | Multiview Stereo with Cascaded Epipolar RAFT   <br> <sub><sup>*Ma, Zeyu and Teed, Zachary and Deng, Jia*</sup></sub> | [Paper](https://link.springer.com/chapter/10.1007/978-3-031-19821-2_42)/[Code](https://github.com/princeton-vl/CER-MVS)
| 2022 | ECCV | MVSTER: Epipolar Transformer for Efficient Multi-View Stereo   <br> <sub><sup>*Xiaofeng Wang, Zheng Zhu, Fangbo Qin, Yun Ye, Guan Huang, Xu Chi, Yijia He, Xingang Wang*</sup></sub> | [Paper](https://arxiv.org/abs/2204.07346)/[Code](https://github.com/JeffWang987/MVSTER)
| 2022 | PAMI | A Survey on Deep Learning Techniques for Stereo-Based Depth Estimation  <br> <sub><sup>*H Laga, LV Jospin, F Boussaid, M Bennamoun*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/9233988)
| 2021 | CVPR | PatchmatchNet: Learned Multi-View Patchmatch Stereo  <br> <sub><sup>*Fangjinhua Wang and Silvano Galliani and Christoph Vogel and Pablo Speciale and Marc Pollefeys*</sup></sub> | [Paper](https://openaccess.thecvf.com/content/CVPR2021/html/Wang_PatchmatchNet_Learned_Multi-View_Patchmatch_Stereo_CVPR_2021_paper.html)/[Code](https://github.com/FangjinhuaWang/PatchmatchNet)
| 2021 | PAMI | Visibility-Aware Point-Based Multi-View Stereo Network   <br> <sub><sup>*Chen, Rui and Han, Songfang and Xu, Jing and Su, Hao*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/9076298)/[Code](https://github.com/callmeray/PointMVSNet)
| 2021 | <sup><sub>ISPRS JPRS</sub></sup> | Attention aware cost volume pyramid based multi-view stereo network for 3D reconstruction   <br> <sub><sup>*Anzhu Yu, Wenyue Guo, Bing Liu, Xin Chen, Xin Wang, Xuefeng Cao, Bingchuan Jiang*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/pii/S0924271621000794)/[Code](https://github.com/ArthasMil/AACVP-MVSNet)
| 2021 | <sup><sub>ISPRS JPRS</sub></sup> | Automatic 3D building reconstruction from multi-view aerial images with deep learning <br> <sub><sup>*Dawen Yu, Shunping Ji, Jin Liu, Shiqing Wei*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/pii/S092427162030318X)/[Code](https://gpcv.whu.edu.cn/data)
| 2021 | <sup><sub>ISPRS JPRS</sub></sup> | IMGTR: Image-triangle based multi-view 3D reconstruction for urban scenes  <br> <sub><sup>*Zhihua Hu, Yaolin Hou, Pengjie Tao, Jie Shan*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271621002410)
| 2021 | Displays | Multi-view stereo in the Deep Learning Era: A comprehensive review   <br> <sub><sup>*Xiang Wang, Chen Wang, Bing Liu, Xiaoqing Zhou, Liang Zhang, Jin Zheng, Xiao Bai*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0141938221001062)
| 2020 | CVPR | BlendedMVS: A Large-scale Dataset for Generalized Multi-view Stereo Networks  <br> <sub><sup>*Yao, Yao and Luo, Zixin and Li, Shiwei and Zhang, Jingyang and Ren, Yufan and Zhou, Lei and Fang, Tian and Quan, Long*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_CVPR_2020/html/Yao_BlendedMVS_A_Large-Scale_Dataset_for_Generalized_Multi-View_Stereo_Networks_CVPR_2020_paper.html)/[Code](https://github.com/YoYo000/BlendedMVS)
| 2020 | CVPR | Cascade Cost Volume for High-Resolution Multi-View Stereo and Stereo Matching   <br> <sub><sup>*Xiaodong Gu, Zhiwen Fan, Zuozhuo Dai, Siyu Zhu, Feitong Tan, Ping Tan*</sup></sub> | [Paper](https://arxiv.org/abs/1912.06378)/[Code](https://github.com/kwea123/CasMVSNet_pl)
| 2020 | CVPR | Cost Volume Pyramid Based Depth Inference for Multi-View Stereo  <br> <sub><sup>*Yang, Jiayu and Mao, Wei and Alvarez, Jose M. and Liu, Miaomiao*</sup></sub> | [Paper](https://arxiv.org/abs/1912.08329)/[Code](https://github.com/JiayuYANG/CVP-MVSNet)
| 2020 | <sup><sub>ISPRS JPRS</sub></sup> | Pruning multi-view stereo net for efficient 3D reconstruction  <br> <sub><sup>*Xiang Xiang, Zhiyuan Wang, Shanshan Lao, Baochang Zhang*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271620301763)
| 2019 | ICCV | Point-based Multi-view Stereo Network  <br> <sub><sup>*Chen, Rui and Han, Songfang and Xu, Jing and Su, Hao*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_ICCV_2019/html/Chen_Point-Based_Multi-View_Stereo_Network_ICCV_2019_paper.html)/[Code](https://github.com/callmeray/PointMVSNet)
| 2019 | CVPR | GA-Net: Guided Aggregation Net for End-To-End Stereo Matching  <br> <sub><sup>*Feihu Zhang, Victor Prisacariu, Ruigang Yang, Philip H.S. Torr*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_CVPR_2019/html/Zhang_GA-Net_Guided_Aggregation_Net_for_End-To-End_Stereo_Matching_CVPR_2019_paper.html)/[Code](https://github.com/feihuzhang/GANet)
| 2019 | CVPR | Recurrent MVSNet for High-resolution Multi-view Stereo Depth Inference  <br> <sub><sup>*Yao, Yao and Luo, Zixin and Li, Shiwei and Shen, Tianwei and Fang, Tian and Quan, Long*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_CVPR_2019/html/Yao_Recurrent_MVSNet_for_High-Resolution_Multi-View_Stereo_Depth_Inference_CVPR_2019_paper.html)/[Code](https://github.com/YoYo000/MVSNet)
| 2018 | ECCV | Specular-to-diffuse translation for multi-view reconstruction  <br> <sub><sup>*Shihao Wu, Hui Huang, Tiziano Portenier, Matan Sela, Daniel Cohen-Or, Ron Kimmel, Matthias Zwicker*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_ECCV_2018/html/Shihao_Wu_Specular-to-Diffuse_Translation_for_ECCV_2018_paper.html)
| 2018 | ECCV | MVSNet: Depth inference for unstructured multi-view stereo    <br> <sub><sup>*Yao Yao, Zixin Luo, Shiwei Li, Tian Fang, Long Quan*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_ECCV_2018/html/Yao_Yao_MVSNet_Depth_Inference_ECCV_2018_paper.html)/[Code](https://github.com/YoYo000/MVSNet)
| 2018 | CVPR | DeepMVS: Learning Multi-View Stereopsis   <br> <sub><sup>*Po-Han Huang, Kevin Matzen, Johannes Kopf, Narendra Ahuja, Jia-Bin Huang*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_cvpr_2018/html/Huang_DeepMVS_Learning_Multi-View_CVPR_2018_paper.html)/[Code](https://phuang17.github.io/DeepMVS/)
| 2017 | ICCV | Monocular Dense 3D Reconstruction of a Complex Dynamic Scene From Two Perspective Frames    <br> <sub><sup>*Suryansh Kumar, Yuchao Dai, Hongdong Li*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_iccv_2017/html/Kumar_Monocular_Dense_3D_ICCV_2017_paper.html)
| 2017 | ICCV | Surfacenet: An end-to-end 3d neural network for multiview stereopsis <br> <sub><sup>*Mengqi Ji, Juergen Gall, Haitian Zheng, Yebin Liu, Lu Fang*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_iccv_2017/html/Ji_SurfaceNet_An_End-To-End_ICCV_2017_paper.html)/[Code](https://github.com/mjiUST/SurfaceNet)
| 2017 | ICCV | End-To-End Learning of Geometry and Context for Deep Stereo Regression   <br> <sub><sup>*Alex Kendall, Hayk Martirosyan, Saumitro Dasgupta, Peter Henry, Ryan Kennedy, Abraham Bachrach, Adam Bry*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_iccv_2017/html/Kendall_End-To-End_Learning_of_ICCV_2017_paper.html)/[Code](https://github.com/MaidouPP/gc_net_stereo)
| 2017 | CVPR | SGM-Nets: Semi-Global Matching With Neural Networks   <br> <sub><sup>*Akihito Seki, Marc Pollefeys*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_cvpr_2017/html/Seki_SGM-Nets_Semi-Global_Matching_CVPR_2017_paper.html)
| 2017 | NeurIPS | Learning a Multi-View Stereo Machine  <br> <sub><sup>*Abhishek Kar, Christian Häne, Jitendra Malik*</sup></sub> | [Paper](https://proceedings.neurips.cc/paper_files/paper/2017/hash/9c838d2e45b2ad1094d42f4ef36764f6-Abstract.html)/[Code](https://github.com/akar43/lsm)
| 2016 | JMLR | Stereo matching by training a convolutional neural network to compare image patches   <br> <sub><sup>*Zbontar, Jure and LeCun, Yann*</sup></sub> | [Paper](https://arxiv.org/abs/1510.05970)/[Code](https://github.com/jzbontar/mc-cnn)
| 2016 | TGRS | Hierarchical and adaptive phase correlation for precise disparity estimation of UAV images   <br> <sub><sup>*Jie Li; Yiguang Liu; Shuangli Du; Pengfei Wu; Zhenyu Xu*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/7547934)
| 2016 | RS | Multi-view stereo matching based on self-adaptive patch and image grouping for multiple unmanned aerial vehicle imagery   <br> <sub><sup>*Xiao, Xiongwu and Guo, Bingxuan and Li, Deren and Li, Linhui and Yang, Nan and Liu, Jianchen and Zhang, Peng and Peng, Zhe*</sup></sub> | [Paper](https://www.mdpi.com/2072-4292/8/2/89)
| 2015 | CGV | Multi-view stereo: A tutorial    <br> <sub><sup>*Yasutaka Furukawa and Carlos Hernández*</sup></sub> | [Paper](https://www.nowpublishers.com/article/Details/CGV-052)
| 2015 | ICCV | Massively Parallel Multiview Stereopsis by Surface Normal Diffusion  <br> <sub><sup>*Silvano Galliani, Katrin Lasinger, Konrad Schindler*</sup></sub> | [Paper](https://openaccess.thecvf.com/content_iccv_2015/html/Galliani_Massively_Parallel_Multiview_ICCV_2015_paper.html)
| 2014 | PhotoRec | State of the art in high density image matching    <br> <sub><sup>*Fabio Remondino, Maria Grazia Spera, Erica Nocerino, Fabio Menna, Francesco Nex*</sup></sub> | [Paper](https://onlinelibrary.wiley.com/doi/abs/10.1111/phor.12063)
| 2014 | AppGeo | UAV for 3D mapping applications: a review  <br> <sub><sup>*Francesco Nex & Fabio Remondino*</sup></sub> | [Paper](https://link.springer.com/article/10.1007/s12518-013-0120-x)
| 2012 | RS | Assessing the accuracy of georeferenced point clouds produced via multi-view stereopsis from unmanned aerial vehicle (UAV) imagery <br> <sub><sup>*Steve Harwin and Arko Lucieer*</sup></sub> | [Paper](https://www.mdpi.com/2072-4292/4/6/1573)



:small_orange_diamond: **MVS Toolkit** 

| **Name** | **Year** | **Pub**          | 
| :------ | :------: | :----------------------------------------------------------- |  
| [Meshroom](https://github.com/alicevision/meshroom) | 2021 | [MMSys](https://dl.acm.org/doi/10.1145/3458305.3478443)
| [Colmap](https://github.com/colmap/colmap) | 2016 | [CVPR](https://www.cv-foundation.org/openaccess/content_cvpr_2016/html/Schonberger_Structure-From-Motion_Revisited_CVPR_2016_paper.html)
| [MicMac](https://github.com/micmacIGN/micmac) | -- | 
| [MVE](https://github.com/simonfuhrmann/mve) | 2014 | [Paper](https://diglib.eg.org/handle/10.2312/gch.20141299.011-018)
| [MVS-Texturing](https://github.com/nmoehrle/mvs-texturing) | 2014 | [ECCV](https://link.springer.com/chapter/10.1007/978-3-319-10602-1_54) 
| [CMVS-PMVS](https://github.com/pmoulon/CMVS-PMVS) | 2010 | [PAMI](https://ieeexplore.ieee.org/abstract/document/5226635)/[Homepage](https://www.di.ens.fr/cmvs/)
| [S2P - Satellite Stereo Pipeline](https://github.com/centreborelli/s2p) | 2014 | 
| [SAT-PP](http://www.4dixplorer.com/software_satpp.html) | | 
| [Danesfield](https://github.com/Kitware/Danesfield) | 2019 | [CVPRW](https://openaccess.thecvf.com/content_CVPRW_2019/html/EarthVision/Leotta_Urban_Semantic_3D_Reconstruction_From_Multiview_Satellite_Imagery_CVPRW_2019_paper.html)



### 7. Image stitching

- [Awesome-Computational-Photography](https://github.com/visionxiang/awesome-computational-photography#Image-Stitching)


| **Year** | **Pub.** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- | 
| 2022 | GRSL | Efficient Seamline Network Generation for Large-Scale Orthoimage Mosaicking  <br> <sub><sup>*Junxing Yang; Lulu Liu; Qingsong Yan; Fei Deng*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/9754551)
| 2021 | TGRS | Superpixel-Based Seamless Image Stitching for UAV Images   <br> <sub><sup>*Yiting Yuan; Faming Fang; Guixu Zhang*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/9115682)
| 2021 | JSTARS | An Efficient Method for Generating UAV-Based Hyperspectral Mosaics Using Push-Broom Sensors  <br> <sub><sup>*Juan M. Jurado; Luís Pádua; Jonas Hruška; Francisco R. Feito; et al*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/9454354)
| 2020 | <sup><sub>ISPRS JPRS</sub></sup> | Jointly optimizing global and local color consistency for multiple image mosaicking   <br> <sub><sup>*Li Li, Menghan Xi, Chi Liu, Liang Li, Hanyun Wang, Jian Yao*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271620302781)
| 2020 | JSTARS | UAV Image Mosaicking Based on Multiregion Guided Local Projection Deformation  <br> <sub><sup>*Quan Xu; Jun Chen; Linbo Luo; Wenping Gong; Yong Wang*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/9130864)
| 2019 | GRSM | Remote Sensing Image Mosaicking: Achievements and Challenges  <br> <sub><sup>*Xinghua Li; Ruitao Feng; Xiaobin Guan; Huanfeng Shen; Liangpei Zhang*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/8937068)
|   2018   |   ECCV   | Object-centered image stitching     <br> <sub><sup>*Charles Herrmann, Ramin Zabih, et al*</sup><sub>  |  [Paper](https://openaccess.thecvf.com/content_ECCV_2018/papers/Charles_Herrmann_Object-centered_image_stitching_ECCV_2018_paper.pdf)/Code      |
|   2018   |   ECCV   | Robust image stitching with multiple registrations    <br> <sub><sup>*Herrmann, Charles, Zabih, Ramin, et al*</sup><sub>  | [Paper](https://openaccess.thecvf.com/content_ECCV_2018/papers/Charles_Herrmann_Robust_image_stitching_ECCV_2018_paper.pdf)/Code   |
|   2018   |   TIP    | Dynamic Video Stitching via Shakiness Removing               <br> <sub><sup>*Yongwei Nie, et al*</sup><sub>               | [Paper](https://ieeexplore.ieee.org/document/8003352)/[Code](https://github.com/SuTanTank/VideoStitchingViaShakinessRemoving) |
| 2018 | RAL | Unsupervised Deep Homography: A Fast and Robust Homography Estimation Model   <br> <sub><sup>*Ty Nguyen; Steven W. Chen; Shreyas S. Shivakumar; Camillo Jose Taylor; Vijay Kumar*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/8302515)/[Code](https://github.com/tynguyen/unsupervisedDeepHomographyRAL2018)
| 2018 | PR | Image stitching by line-guided local warping with global similarity constraint   <br> <sub><sup>*Tian-Zhu Xiang, Gui-Song Xia, Xiang Bai, Liangpei Zhang*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0031320318302231)
| 2018 | TMM | Parallax-Tolerant Image Stitching Based on Robust Elastic Warping   <br> <sub><sup>*Jing Li; Zhengming Wang; Shiming Lai; Yongping Zhai; Maojun Zhang*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/8119833)/[Code](https://github.com/gain2217/Robust_Elastic_Warping)
|   2018   |   TMM    | Quasi-Homography Warps in Image Stitching    <br> <sub><sup>*Nan Li, Yifang Xu, Chao Wang*</sup><sub>   |  [Paper](https://ieeexplore.ieee.org/document/8101022)/Code   |
| 2018 | IJRS | Mosaicking UAV orthoimages using bounded Voronoi diagrams and watersheds   <br> <sub><sup>*Mengxiao Song, Zheng Ji, Shan Huang &Jing Fu*</sup></sub> | [Paper](https://www.tandfonline.com/doi/abs/10.1080/01431161.2017.1350309)
| 2018 | IJRS | Seam-line determination via minimal connected area searching and minimum spanning tree for UAV image mosaicking <br> <sub><sup>*Yumin Tian,Aifeng Sun &Di Wang*</sup></sub> | [Paper](https://www.tandfonline.com/doi/abs/10.1080/01431161.2017.1420939)
| 2017 |  CVPR  | Direct Photometric Alignment by Mesh Deformation             <br> <sub><sup>*Kaimo Lin, Shuaicheng Liu, et al*</sup><sub>   | [Paper](https://openaccess.thecvf.com/content_cvpr_2017/papers/Lin_Direct_Photometric_Alignment_CVPR_2017_paper.pdf)/[Code](https://github.com/lxlscut/optical2.0)  |
| 2017 | PR | Globally consistent alignment for planar mosaicking via topology analysis  <br> <sub><sup>*Menghan Xia, Jian Yao, Renping Xie, Li Li, Wei Zhang*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0031320317300201)
| 2017 | AutCon | UAV-based automatic generation of high-resolution panorama at a construction site with a focus on preprocessing for image stitching   <br> <sub><sup>*Seongdeok Bang, Hongjo Kim, Hyoungkwan Kim*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0926580517301929)
| 2016 | ECCV | Natural Image Stitching with the Global Similarity Prior  <br> <sub><sup>*Yu-Sheng Chen & Yung-Yu Chuang*</sup></sub> | [Paper](https://link.springer.com/chapter/10.1007/978-3-319-46454-1_12)/[Code](https://github.com/nothinglo/NISwGSP)
| 2016 | ECCV | SEAGULL: Seam-Guided Local Alignment for Parallax-Tolerant Image Stitching   <br> <sub><sup>*Kaimo Lin, Nianjuan Jiang, Loong-Fah Cheong, Minh Do & Jiangbo Lu*</sup></sub> | [Paper](https://link.springer.com/chapter/10.1007/978-3-319-46487-9_23)
| 2016 | TIP | Multi-viewpoint panorama construction with wide-baseline images   <br> <sub><sup>*Guofeng Zhang; Yi He; Weifeng Chen; Jiaya Jia; Hujun Bao*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/7420659)
| 2016 | RS | Mosaicking of Unmanned Aerial Vehicle Imagery in the Absence of Camera Poses   <br> <sub><sup>*Yuhua Xu, Jianliang Ou, Hu He, Xiaohu Zhang and Jon Mills*</sup></sub> | [Paper](https://www.mdpi.com/2072-4292/8/3/204)/[Code](https://github.com/YuhuaXu/ImageMosaicing)
| 2016 |   RSS-W   |  Deep Image Homography Estimation   <br> <sub><sup>*Daniel DeTone, et al*</sup><sub>  | [Paper](https://arxiv.org/abs/1606.03798)/[Code](https://github.com/mazenmel/Deep-homography-estimation-Pytorch)
| 2016 | JARS | Computer vision-based orthorectification and georeferencing of aerial image sets   <br> <sub><sup>*Mohammad Reza Faraji, Xiaojun Qi, Austin Jensen*</sup></sub> | [Paper](https://www.spiedigitallibrary.org/journals/journal-of-applied-remote-sensing/volume-10/issue-3/036027/Computer-visionbased-orthorectification-and-georeferencing-of-aerial-image-sets/10.1117/1.JRS.10.036027.short?SSO=1)
| 2016 | Sensors | An Efficient Seam Elimination Method for UAV Images Based on Wallis Dodging and Gaussian Distance Weight Enhancement   <br> <sub><sup>*Jinyan Tian, Xiaojuan Li, Fuzhou Duan, Junqian Wang and Yang Ou*</sup></sub> | [Paper](https://www.mdpi.com/1424-8220/16/5/662)
| 2016 | ICPR | Locally warping-based image stitching by imposing line constraints  <br> <sub><sup>*T.-Z. Xiang, G.-S. Xia, L. Zhang, and N. Huang*</sup></sub> | [Paper](https://ieeexplore.ieee.org/abstract/document/7900289)
|   2015   |   ICCV   |  Dual-Feature Warping-Based Motion Model Estimation  <br> <sub><sup>*Shiwei Li, Lu Yuan, Jian Sun, Long Quan*</sup><sub> | [Paper](https://openaccess.thecvf.com/content_iccv_2015/html/Li_Dual-Feature_Warping-Based_Motion_ICCV_2015_paper.html)/Code
|   2015   |   CVPR   | Adaptive As-Natural-As-Possible Image Stitching  <br> <sub><sup>*Chung-Ching Lin, S. U. Pankanti, K. N. Ramamurthy, and Aleksandr Y. Aravkin*</sup><sub> | [Paper](https://openaccess.thecvf.com/content_cvpr_2015/papers/Lin_Adaptive_As-Natural-As-Possible_Image_2015_CVPR_paper.pdf)/[Code](https://github.com/YaqiLYU/AANAP)
| 2015 | <sup><sub>ISPRS JPRS</sub></sup> | A robust mosaicking procedure for high spatial resolution remote sensing images     <br> <sub><sup>*Xinghua Li, Nian Hui, Huanfeng Shen, Yunjie Fu, Liangpei Zhang*</sup></sub> | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271615002191)
| 2015 | CluCom | A review of parallel computing for large-scale remote sensing image mosaicking   <br> <sub><sup>*Lajiao Chen, Yan Ma, Peng Liu, Jingbo Wei, Wei Jie & Jijun He*</sup><sub> | [Paper](https://link.springer.com/article/10.1007/s10586-015-0422-3)
| 2014 |   CVPR   |  Shape-preserving half-projective warps for image stitching <br> <sub><sup>*Che-Han Chang, Yoichi Sato, Yung-Yu Chuang*</sup><sub> | [Paper](https://www.cv-foundation.org/openaccess/content_cvpr_2014/html/Chang_Shape-Preserving_Half-Projective_Warps_2014_CVPR_paper.html)/Code
| 2014 |   CVPR  |  Parallax-tolerant Image Stitching  <br> <sub><sup>*Fan Zhang and Feng Liu*</sup><sub>  | [Paper](https://openaccess.thecvf.com/content_cvpr_2014/papers/Zhang_Parallax-tolerant_Image_Stitching_2014_CVPR_paper.pdf)
| 2014 | PAMI | As-Projective-As-Possible Image Stitching with Moving DLT  <br> <sub><sup>*Julio Zaragoza; Tat-Jun Chin; Quoc-Huy Tran; Michael S. Brown; David Suter*</sup></sub> | [Paper](https://ieeexplore.ieee.org/document/6682890)/[Code](https://cs.adelaide.edu.au/~tjchin/apap/)/<br>[Code](https://github.com/EadCat/APAP-Image-Stitching)
|   2013   |  EG | Seam-Driven Image Stitching   <br> <sub><sup>*Junhong Gao, Yu Li, Tat-Jun Chin, Michael S. Brown*</sup><sub>  |  [Paper](https://yu-li.github.io/paper/eg13_stitching.pdf)/Code
|   2011   | CVPR  | Smoothly varying affine stitching   <br> <sub><sup>*Wen-Yan Lin, Siying Liu, Y Matsushita, Tian-Tsong Ng, Loong-Fah Cheong*</sup><sub>  | [Paper](https://ieeexplore.ieee.org/document/5995314)/[Code](https://sites.google.com/site/laoszefei81/home/code-1/code-for-smoothly-varying-affine-stitching)
|   2011   | CVPR | Constructing image panoramas using dual-homography warping <br> <sub><sup>*Junhong Gao, Seon Joo Kim, Michael S. Brown*</sup><sub>   | [Paper](https://ieeexplore.ieee.org/document/5995433)/Code
|   2007  |  IJCV | Automatic panoramic image stitching using invariant features <br> <sub><sup>*Matthew Brown and David G. Lowe*</sup><sub>  | [Paper](http://matthewalunbrown.com/papers/ijcv2007.pdf)/[Demo](http://matthewalunbrown.com/autostitch/autostitch.html)
| 2007 | CGV | Image Alignment and Stitching: A Tutorial  <br> <sub><sup>*Rick Szeliski*</sup></sub> | [Paper](https://www.nowpublishers.com/article/Details/CGV-009)



:small_orange_diamond: **Stitching Toolkit** 
 
- [Image composition editor (ICE)](https://www.microsoft.com/en-us/research/project/image-composite-editor/)
- [Autostitch](http://matthewalunbrown.com/autostitch/autostitch.html)



### 8. Multi-sensor data registration


:small_orange_diamond: **Multi-band image registration** 


| **Year** | **Pub.** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- | 
| 2024 | InfFus | POS-GIFT: A Geometric and Intensity-Invariant Feature Transformation for Multimodal Images   <br> <sub><sup>*Zhuolu Hou, Yuxuan Liu, Li Zhang*</sup><sub>  | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S1566253523003433)/[Code](https://github.com/Zhuolu-Hou/POS-GIFT)
| 2023 | <sup><sub>ISPRS JPRS</sub></sup> | Multimodal image matching: A scale-invariant algorithm and an open dataset  <br> <sub><sup>*Jiayuan Li, Qingwu Hu, Yongjun Zhang*</sup><sub>  | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271623002277)/[Code](https://github.com/LJY-RS/SRIF/tree/master)
| 2023 | InfFus | Shape-Former: Bridging CNN and Transformer via ShapeConv for multimodal image matching   <br> <sub><sup>*Jiaxuan Chen, Xiaoxian Chen, Shuang Chen, Yuyan Liu, et al*</sup><sub>  | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S1566253522002068)
| 2023 | JMASS | Advances and Challenges in Multimodal Remote Sensing Image Registration   <br> <sub><sup>*Bai Zhu; Liang Zhou; Simiao Pu; Jianwei Fan; Yuanxin Ye*</sup><sub>  | [Paper](https://ieeexplore.ieee.org/abstract/document/10044278)
| 2022 | <sup><sub>ISPRS JPRS</sub></sup> | A robust multimodal remote sensing image registration method and system using steerable filters with first- and second-order gradients   <br> <sub><sup>*Yuanxin Ye, Bai Zhu, Tengfeng Tang, Chao Yang, Qizhi Xu, Guo Zhang*</sup><sub>  | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271622001083)/[Code](https://github.com/yeyuanxin110/SFOC-Multimodal_Remote_Sensing_Image_Registration_System)
| 2022 | <sup><sub>ISPRS JPRS</sub></sup> | A robust registration method for UAV thermal infrared and visible images taken by dual-cameras  <br> <sub><sup>*Lingxuan Meng, Ji Zhou, Shaomin Liu, Ziwei Wang, et al*</sup><sub>  | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271622002271)/[Code](https://github.com/mlxljz/TWMM)
| 2022 | TGRS | A Multiscale Framework With Unsupervised Learning for Remote Sensing Image Registration  <br> <sub><sup>*Yuanxin Ye; Tengfeng Tang; Bai Zhu; Chao Yang; Bo Li; et al*</sup><sub>  | [Paper](https://ieeexplore.ieee.org/abstract/document/9758703)/[Code](https://github.com/yeyuanxin110/MU-Net/tree/main)
| 2022 | TGRS | LNIFT: Locally Normalized Image for Rotation Invariant Multimodal Feature Matching   <br> <sub><sup>*Jiayuan Li; Wangyi Xu; Pengcheng Shi; Yongjun Zhang; Qingwu Hu*</sup><sub>  | [Paper](https://ieeexplore.ieee.org/abstract/document/9751712)/[Code](https://github.com/LJY-RS/LNIFT_matlab)
| 2021 | JSTARS | Self-Similarity Features for Multimodal Remote Sensing Image Matching   <br> <sub><sup>*Xin Xiong; Guowang Jin; Qing Xu; Hongmin Zhang*</sup><sub>  | [Paper](https://ieeexplore.ieee.org/abstract/document/9629297)
| 2021 | GRSM | Advances and Opportunities in Remote Sensing Image Geometric Registration: A systematic review of state-of-the-art approaches and future research directions   <br> <sub><sup>*Ruitao Feng; Huanfeng Shen; Jianjun Bai; Xinghua Li*</sup><sub>  | [Paper](https://ieeexplore.ieee.org/abstract/document/9468875)
| 2021 | RS | Multimodal Remote Sensing Image Registration Methods and Advancements: A Survey   <br> <sub><sup>*Xinyue Zhang, Chengcai Leng, Yameng Hong, Zhao Pei, Irene Cheng and Anup Basu*</sup><sub>  | [Paper](https://www.mdpi.com/2072-4292/13/24/5128)
| 2021 | IJRS | A comprehensive review on remote sensing image registration     <br> <sub><sup>*Sourabh Paul &Umesh C. Pati*</sup><sub>  | [Paper](https://www.tandfonline.com/doi/abs/10.1080/01431161.2021.1906985)
| 2021 | InfFus | A review of multimodal image matching: Methods and applications  <br> <sub><sup>*Xingyu Jiang, Jiayi Ma, Guobao Xiao, Zhenfeng Shao, Xiaojie Guo*</sup><sub>  | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S156625352100035X)
| 2019 | TIP | RIFT: Multi-Modal Image Matching Based on Radiation-Variation Insensitive Feature Transform   <br> <sub><sup>*Jiayuan Li; Qingwu Hu; Mingyao Ai*</sup><sub>  | [Paper](https://ieeexplore.ieee.org/abstract/document/8935498)/[Code](https://github.com/LJY-RS/RIFT-multimodal-image-matching)
| 2019 | <sup><sub>ISPRS JPRS</sub></sup> | Robust registration for remote sensing images by combining and localizing feature- and area-based methods  <br> <sub><sup>*Ruitao Feng, Qingyun Du, Xinghua Li, Huanfeng Shen*</sup><sub>  | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271619300632)
| 2019 | TGRS | Fast and Robust Matching for Multimodal Remote Sensing Image Registration  <br> <sub><sup>*Yuanxin Ye; Lorenzo Bruzzone; Jie Shan; Francesca Bovolo, Qing Zhu*</sup><sub>  | [Paper](https://ieeexplore.ieee.org/abstract/document/8766118)/[Code](https://github.com/yeyuanxin110/CFOG)
| 2019 | JSTARS | Registration of Multimodal Remote Sensing Image Based on Deep Fully Convolutional Neural Network  <br> <sub><sup>*Han Zhang; Weiping Ni; Weidong Yan; Deliang Xiang, et al*</sup><sub>  | [Paper](https://ieeexplore.ieee.org/abstract/document/8730416)
| 2019 | PRL | Robust visible infrared image matching by exploiting dominant edge orientations   <br> <sub><sup>*H. Chen, N. Xue, Y. Zhang, Q. Lu, and G.-S. Xia*</sup><sub>  | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0167865518308651)
| 2018 | TGRS | Robust registration of multimodal remote sensing images based on structural similarity   <br> <sub><sup>*Yuanxin Ye; Jie Shan; Lorenzo Bruzzone; Li Shen*</sup><sub>  | [Paper](https://ieeexplore.ieee.org/abstract/document/7862734)/[Code](https://github.com/yeyuanxin110/HOPC)
| 2015 | <sup><sub>ISPRS JPRS</sub></sup> | A fast and mobile system for registration of low-altitude visual and thermal aerial images using multiple small-scale UAVs  <br> <sub><sup>*S. Yahyanejad and B. Rinner*</sup><sub>  | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271614001993)
| 2013 | PRL | Visible and infrared image registration in man-made environments employing hybrid visual features  <br> <sub><sup>*Jungong Han, Eric J. Pauwels, Paul de Zeeuw*</sup><sub>  | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0167865512001043)
| 2008 | PR | Multi-sensor image registration based on intensity and edge orientation information  <br> <sub><sup>*Yong Sun Kim, Jae Hak Lee, Jong Beom Ra*</sup><sub>  | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0031320308001684)



:small_orange_diamond: **Registration of LiDAR and optical images**

| **Year** | **Pub.** | **Title**          | **Links**        |
| :------: | :------: | :----------------------------------------------------------- |  :----------------------------------------------------------- |
| 2021 | <sup><sub>ISPRS JPRS</sub></sup> | Robust registration of aerial images and LiDAR data using spatial constraints and Gabor structural features  <br> <sub><sup>*Bai Zhu, Yuanxin Ye, Liang Zhou, Zhilin Li, Gaofei Yin*</sup><sub>  | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271621002422)
| 2019 | <sup><sub>ISPRS JPRS</sub></sup> | NRLI-UAV: Non-rigid registration of sequential raw laser scans and images for low-cost UAV LiDAR point cloud quality improvement    <br> <sub><sup>*Jianping Li, Bisheng Yang, Chi Chen, Ayman Habib*</sup><sub>  | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271619302473)
| 2019 | <sup><sub>ISPRS JPRS</sub></sup> | Marker-free coregistration of UAV and backpack LiDAR point clouds in forested areas    <br> <sub><sup>*Przemyslaw Polewski a, Wei Yao a, Lin Cao b, Sha Gao*</sup><sub>  | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S092427161830323X)
| 2016 | RS | A linear feature-based approach for the registration of unmanned aerial vehicle remotely-sensed images and airborne LiDAR data  <br> <sub><sup>*S. Liu, X. Tong, J. Chen, X. Liu, W. Sun, H. Xie, P. Chen, Y. Jin, and Z. Ye*</sup><sub>  | [Paper](https://www.mdpi.com/2072-4292/8/2/82)
| 2015 | <sup><sub>ISPRS JPRS</sub></sup>  | Automatic registration of UAV-borne sequent images and LiDAR data  <br> <sub><sup>*Bisheng Yang and Chi Chen*</sup><sub>  | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271615000180)
| 2015 | <sup><sub>ISPRS JPRS</sub></sup>  | Automatic registration of optical aerial imagery to a LiDAR point cloud for generation of city models  <br> <sub><sup>*Bernard O. Abayowa, Alper Yilmaz, Russell C. Hardie*</sup><sub>  | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271615001434)



## Dataset and Tools 

:small_orange_diamond: **Tools** 

- [awesome-photogrammetry-projects](https://github.com/awesome-photogrammetry/awesome-photogrammetry)


| **Name** | **Year** |  **Links** | **Comments** | 
| :------ | :------: | :----------------------- | :----------------------- |
| [OpenDroneMap](https://www.opendronemap.org/) | -- | [Github](https://github.com/OpenDroneMap/ODM) | <sub><sup>An open source command line toolkit for processing aerial drone imagery to generate maps, point clouds, 3D models and DEMs</sup></sub>
| [VisWebDrone](https://github.com/Nathalieguimaraes/VisWebDrone) | 2020 | [IJGI](https://www.mdpi.com/2220-9964/9/11/679) | <sub><sup>A web application for photogrammetric processing</sup></sub>
| [TeleSculptor](https://github.com/Kitware/TeleSculptor) | -- | -- |  <sub><sup>A cross-platform desktop application for aerial photogrammetry</sup></sub>
| [CloudCompare](https://www.cloudcompare.org/) | -- | -- | <sub><sup>3D point cloud and mesh processing software</sup></sub>



:small_orange_diamond: **Dataset** 

| **Name** | **Year** | **Comments** | 
| :------ | :------: | :----------------------- |
| [SUIRD](https://github.com/yyangynu/SUIRD) | 2019 | <sub><sup>Small UAV Image Registration Dataset (SUIRD)</sup></sub> 
| [Urban Drone Dataset (UDD)](https://github.com/MarcWong/SemanticSfM/tree/master/dataset) | 2018 | <sub><sup>Structure from Motion of Aerial Images ([PRCV](https://link.springer.com/chapter/10.1007/978-3-030-03398-9_30))</sup></sub>
| [UAV image mosaicking dataset](https://github.com/YuhuaXu/UAV-image-mosaicing-dataset) | 2016 | <sub><sup>Dataset for Unmanned Aerial Vehicle (UAV) Image Mosaicking ([RS](https://www.mdpi.com/2072-4292/8/3/204))</sup></sub>
| [ISPRS/EuroSDR Benchmark for <br>Multi-Platform Photogrammetry](https://www2.isprs.org/commissions/comm2/icwg-2-1a/benchmark_main/) | 2015 | <sub><sup>For dense Image Matching and Image Orientation</sup></sub>
| [Benchmark on High Density <br>Aerial Image Matching](https://ifpwww.ifp.uni-stuttgart.de/ISPRS-EuroSDR/ImageMatching/default.aspx) | 2015 | <sub><sup>For dense image matching</sup></sub>
| :triangular_flag_on_post: Semantic |  |  |
| [InsPLAD](https://github.com/andreluizbvs/InsPLAD) | 2023 | <sub><sup>Inspection of Power Line Assets: the Dataset (InsPLAD) ([Paper](https://arxiv.org/abs/2311.01619)) </sup></sub> 
| [HIT-UAV](https://github.com/suojiashun/HIT-UAV-Infrared-Thermal-Dataset) | 2023 | <sub><sup>A high-altitude UAV-based infrared thermal dataset for object detection ([Paper](https://www.nature.com/articles/s41597-023-02066-6)/[Homepage](https://pegasus.ac.cn/))</sup></sub> 
| [UAV-ROD](https://github.com/fengkaibit/UAV-ROD) | 2022 | <sub><sup>Car detection (rotating object detection) dataset for UAV imagery ([NeuroCom](https://www.sciencedirect.com/science/article/abs/pii/S0925231222007676))</sup></sub> 
| [VisDrone](https://github.com/VisDrone/VisDrone-Dataset) | 2021 | <sub><sup>Object detection and tracking from UAV data ([PAMI](https://arxiv.org/abs/2001.06303))</sup></sub> 
| [UAV-Human](https://github.com/sutdcv/UAV-Human) | 2021 | <sub><sup>Human Behavior Understanding with UAVs ([CVPR](https://arxiv.org/abs/2104.00946))</sup></sub> 
| [DAC-SDC](https://github.com/xyzxinyizhang/2018-DAC-System-Design-Contest) | 2021 | <sub><sup>Lower power object detection challenge ([PAMI](https://ieeexplore.ieee.org/abstract/document/8787881))</sup></sub> 
| [UAVid](https://uavid.nl/) | 2020 | <sub><sup>Semantic segmentation dataset for UAV imagery</sup></sub>
| [UAVDT](https://sites.google.com/view/daweidu/projects/uavdt?authuser=0) | 2018 | <sub><sup>Object detection, single object tracking, and multiple object tracking ([ECCV](https://openaccess.thecvf.com/content_ECCV_2018/papers/Dawei_Du_The_Unmanned_Aerial_ECCV_2018_paper.pdf ))</sup></sub> 
| [Okutama-Action](http://okutama-action.org/) | 2017 | <sub><sup>Concurrent Human Action Detection ([CVPRW](https://arxiv.org/abs/1706.03038))</sup></sub>
| [UAV123](https://cemse.kaust.edu.sa/ivul/uav123) | 2016 | <sub><sup>Object tracking dataset ([ECCV](https://link.springer.com/chapter/10.1007/978-3-319-46448-0_27))<sub><sup>









## Citation

Please cite our paper if you find the work useful:

```
@article{xiang2019mini,
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

