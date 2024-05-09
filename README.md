# 3D Human Pose SPI

Extracting 3D human pose and body shape details from a single monocular image is a significant challenge in computer vision. Traditional methods use RGB images, constrained by varying lighting and occlusions. However, cutting-edge developments in imaging technologies have introduced new techniques, such as single-pixel imaging (SPI), that can surmount these hurdles. SPI demonstrates impressive capabilities in capturing a 3D human pose in the near-infrared spectrum. This wavelength can penetrate clothing and is less influenced by lighting variations than visible light, thus providing a reliable means to accurately capture body shape and pose data, even in complex settings. This work explores using an SPI camera operating in the NIR with time-of-flight (TOF) at bands 850–1550 nm to detect humans in nighttime environments. The proposed system uses the vision transformers (ViT) model to detect and extract the characteristic features of humans for integration over a 3D body model SMPL-X through 3D body shape regression using deep learning. To evaluate the efficacy of NIR-SPI 3D image reconstruction, we constructed a laboratory scenario that simulates nighttime conditions, enabling us to test the feasibility of employing NIR-SPI as a vision sensor in outdoor environments. By assessing the results obtained from this setup, we aim to demonstrate the potential of NIR-SPI as an effective tool to detect humans in nighttime scenarios and capture their accurate 3D body pose and shape.

![Human_Pose](https://github.com/1Px-Vision/3D_Human_Pose_SPI/assets/150855410/36a021f0-ff5d-4555-a2ce-78040db634a6)

Video
https://opticapublishing.figshare.com/articles/media/3D_Pose_OSA_V1_mp4/24783918

Please check out the following references for more details:

Carlos Osorio Quero, Daniel Durini, Jose Rangel-Magdaleno, Jose Martinez-Carranza, and Ruben Ramos-Garcia, "Enhancing 3D human pose estimation with NIR single-pixel imaging and time-of-flight technology: 
a deep learning approach," J. Opt. Soc. Am. A 41, 414-423 (2024)


Table 1. Various methods have been proposed and evaluated in the competition for estimating 3D human poses from monocular images. These include VIBE (Video Inference for Body pose and shape Estimation), DenseRaC (Dense Reconstruction of Articulated Characters), HoloPose, GCMR (Graph Convolutional Mesh Regression), HMR (Human Mesh Recovery), and UP (Unite the People). Also, the SMPLify algorithm has been considered alongside other methods we have proposed.

| Method  | MPJPE (mm) |Complexity  |Performance|
| ------------- | ------------- |------------- |------------- |
| VIBE  |65.6 |Using a combination of DL and optimization techniques |Offers higher accuracy in dynamic scenarios|
|DenseRaC |76.8 |Significantly complex |Provides detailed and accurate 3D reconstructions|
|HoloPose |60.2 |Aims at high-fidelity 3D human pose estimation |High-quality results may not be ideal for real-time|
|GCMR |71.9 |Employs graph convolutional networks for mesh regression |Performance can be computationally intensive|
|HMR |87.9 |Balances between complexity and efficiency |Good trade-off between accuracy and speed|
|UP |80.7 |Complex depending on the implementation |Offering reliable performance|
|SMPLify |82.3 |Optimization-based approach to fit the SMPL body model |Offers reasonable accuracy in controlled environments|
|Ours |42 |Implementation a strategy of VIT and VIBE methods |3D Reconstructions from Low-Resolution Images|

## Reference
@article{OsorioQuero:24,
author = {Carlos Osorio Quero and Daniel Durini and Jose Rangel-Magdaleno and Jose Martinez-Carranza and Ruben Ramos-Garcia},
journal = {J. Opt. Soc. Am. A},
keywords = {Image metrics; Imaging techniques; Machine vision; Single pixel imaging; Three dimensional imaging; Three dimensional reconstruction},
number = {3},
pages = {414--423},
publisher = {Optica Publishing Group},
title = {Enhancing 3D human pose estimation with NIR single-pixel imaging and time-of-flight technology: a deep learning approach},
volume = {41},
month = {Mar},
year = {2024},
url = {https://opg.optica.org/josaa/abstract.cfm?URI=josaa-41-3-414},
doi = {10.1364/JOSAA.499933},
}
