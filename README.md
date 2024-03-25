# 3D_Human_Pose_SPI

The extraction of 3D human pose and body shape details from a single monocular image is a significant challenge in computer vision. Traditional methods use RGB images, but these are constrained by varying lighting and occlusions. However, cutting-edge developments in imaging technologies have introduced new techniques such as single-pixel imaging (SPI) that can surmount these hurdles. In the near-infrared spectrum, SPI demonstrates impressive capabilities in capturing a 3D human pose. This wavelength can penetrate clothing and is less influenced by lighting variations than visible light, thus providing a reliable means to accurately capture body shape and pose data, even in difficult settings. In this work, we explore the use of an SPI camera operating in the NIR with time-of-flight (TOF) at bands 850–1550 nm as a solution to detect humans in nighttime environments. The proposed system uses the vision transformers (ViT) model to detect and extract the characteristic features of humans for integration over a 3D body model SMPL-X through 3D body shape regression using deep learning. To evaluate the efficacy of NIR-SPI 3D image reconstruction, we constructed a laboratory scenario that simulates nighttime conditions, enabling us to test the feasibility of employing NIR-SPI as a vision sensor in outdoor environments. By assessing the results obtained from this setup, we aim to demonstrate the potential of NIR-SPI as an effective tool to detect humans in nighttime scenarios and capture their accurate 3D body pose and shape.

Video
https://opticapublishing.figshare.com/articles/media/3D_Pose_OSA_V1_mp4/24783918

Carlos Osorio Quero, Daniel Durini, Jose Rangel-Magdaleno, Jose Martinez-Carranza, and Ruben Ramos-Garcia, "Enhancing 3D human pose estimation with NIR single-pixel imaging and time-of-flight technology: 
a deep learning approach," J. Opt. Soc. Am. A 41, 414-423 (2024)

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
