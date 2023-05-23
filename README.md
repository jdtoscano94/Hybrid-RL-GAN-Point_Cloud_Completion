# Teeth Mold Point Cloud Completion Via Data Augmentation and Hybrid RL-GAN (Official Implementation)

![Framework](https://github.com/jdtoscano94/Hybrid-RL-GAN-Point_Cloud_Completion/assets/102500060/c2a68190-3fad-4b49-a597-62f24ee31b62)


## Abstract

Teeth scans are essential for many applications in orthodontics, where the teeth structures
are virtualized to facilitate the design and fabrication of the prosthetic piece. Nevertheless,
due to the limitations caused by factors such as viewing angles, occlusions, and sensor resolution, the 3D scanned point clouds (PCs) could be noisy or incomplete. Hence, a critical need is needed to enhance the teeth' quality to ensure a suitable dental treatment.
Toward this end, we propose a systematic framework including a two-step data augmentation (DA) technique to augment the limited teeth PCs and deep hybrid learning (DL)
method to complete the incomplete PCs. For the two-step DA, we first mirror and
combine the PCs based on the bilateral symmetry of the human teeth and then augment
the PCs based on an iterative generative adversarial network (GAN). Two filters are
designed to avoid the outlier and duplicated PCs during the DA. For the hybrid DL, we
first use a deep autoencoder (AE) to represent the PCs. Then, we propose a hybrid approach
that selects the best completion to the teeth PCs from AE and a reinforcement learning (RL)
agent-controlled GAN. An ablation study is performed to analyze each component's contribution. We compared our method with other benchmark methods, including point cloud
network (PCN), cascaded refinement network (CRN), and variational relational point completion network (VRC-Net). We demonstrated that the proposed framework is suitable for
completing teeth PCs with good accuracy over different scenarios.


### Results
![Results](https://github.com/jdtoscano94/Hybrid-RL-GAN-Point_Cloud_Completion/assets/102500060/b714997e-495b-4de2-aef5-070003c115b2)



Paper: https://asmedigitalcollection.asme.org/computingengineering/article/23/4/041008/1155799/Teeth-Mold-Point-Cloud-Completion-Via-Data

## Components
 - Deep Autoencoders
 - Generative Adversarial Neural Networks
 - Reinforcement Learning
 - Data augmentation algorithms
## Steps
All the models were trained using Google Colab Pro. To reimplement the results, you can follow these steps:
1. Download from: https://drive.google.com/drive/folders/1_VmlWu-_HaWPlK1t5X0ZuMv-YtDEvDE2?usp=sharing
2. Preprocess the data using: 0_Point_Cloud_Preprocessing.ipynb
3. Train the first Autoencoder using: 1_AEMoldScan.ipynb
4. Train the first GAN and filter the generated data using: 2_3_GANMoldScan.ipynb
5. Train the second Autoencoder using: 1_AEMoldScan.ipynb
6. Train the second GAN and filter the generated data using: 2_3_GANMoldScan.ipynb
7. Train the reinforcement learning agent using: 4_RLMoldScan.ipynb
8. Evaluate the results using: 5_Final.ipynb
## Citation
@article{toscano2023teeth,
  title={Teeth Mold Point Cloud Completion Via Data Augmentation and Hybrid RL-GAN},
  author={Toscano, Juan Diego and Zuniga-Navarrete, Christian and Siu, Wilson David Jo and Segura, Luis Javier and Sun, Hongyue},
  journal={Journal of Computing and Information Science in Engineering},
  volume={23},
  number={4},
  pages={041008},
  year={2023},
  publisher={American Society of Mechanical Engineers}
}
## Credits 
1. https://github.com/iSarmad/RL-GAN-Net
2. https://github.com/optas/latent_3d_points
3. https://github.com/heykeetae/Self-Attention-GAN
4. https://github.com/lijx10/SO-Net
5. https://github.com/sfujim/TD3
